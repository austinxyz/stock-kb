---
source: austin
---

# outputs/ — 时间点快照目录

`outputs/` 存放所有**时间点快照（point-in-time snapshots）**：生成后不再修改，记录某一时刻的分析结论或市场状态。

与 `wiki/`（常青内容，随新信息更新）的区别：

| | `wiki/` | `outputs/` |
|---|---|---|
| 性质 | 常青 — 事实变化时更新 | 冻结 — 写完不改 |
| 举例 | 个股论文、ETF 分析、框架 | 入场计划、日报、月报 |
| 来源 | Austin overlay | Upstream (kgajjala) + Austin overlay |

---

## 目录结构

```
outputs/
├── <TICKER>/                          ← 个股快照（upstream + overlay 合并）
│   ├── <TICKER>_initial_analysis_YYYY-MM-DD.md   ← upstream 初始分析（source: upstream）
│   └── entry-YYYY-MM-DD.md                        ← Austin 入场计划（source: austin）
└── market/                            ← 市场报告
    ├── index.md                       ← 日报归档索引（最近 30 条）
    ├── daily/
    │   └── YYYY-MM-DD.md              ← 每日市场报告（source: austin）
    ├── weekly/
    │   └── YYYY-Www.md                ← 每周市场回顾（source: austin）
    ├── monthly/
    │   └── YYYY-MM.md                 ← 每月市场月报（source: austin）
    └── quarterly/
        └── YYYY-Qn.md                 ← 每季市场季报（source: austin）
```

---

## 1. 个股快照 — `outputs/<TICKER>/`

### 1a. Upstream 初始分析（来自 kgajjala/rwh）

**文件名格式：** `<TICKER>_initial_analysis_YYYY-MM-DD.md`

**来源：** `../rwh/outputs/<TICKER>/`，由 upstream 的分析流程生成，经 `kb-sync` 复制到此。

**内容：** 整合了 15 节论文 + 关键财务表格的全量快照。每次 upstream 更新分析后，会新增一个带日期的文件（旧文件保留，形成版本序列）。

**不要手动编辑。** 这是 upstream 的原始输出，覆盖由 `kb-sync` 管理。

**当前覆盖 ticker（来自 upstream）：**
ABNB · ACLS · ADBE · AMZN · BKNG · BRK.B · CELH · CPNG · DASH · DELL · EBAY · FIG · HOOD · INTU · KGS · LLY · LNTH · LULU · MP · MSFT · NFLX · NKE · ONON · PG · RH · RIVN · RKT · SBUX · SCHW · SHOP · SN · SPOT · TREX · TSLA · UNH · WING · ZG（及其他）

### 1b. Austin 入场计划（overlay 扩展）

**文件名格式：** `entry-YYYY-MM-DD.md`

**来源：** `/stock-entry <TICKER>` 命令生成，写入 `outputs/<TICKER>/`。

**内容：** 入场区间、止损位、目标价、仓位规模（按 1% 本金风险）、ATR、期权关键位（max pain / OI 阻力/支撑）。

**生成方式：**
```
/stock-entry POET   → outputs/POET/entry-2026-04-26.md
```

**与 wiki 的关联：**
- `wiki/tickers/<TICKER>/overview.md` 的「历史入场分析」区块维护链接列表
- `wiki/tickers/<TICKER>/changelog.md` 记录每次入场事件

**可与 upstream 共存：** 同一 TICKER 目录下，upstream 的 `_initial_analysis_*` 和 Austin 的 `entry-*` 并排存放。`kb-sync` 用 `source: upstream` / `source: austin` frontmatter 区分来源。

---

## 2. 市场报告 — `outputs/market/`

所有市场报告均由对应 `/market-*` 命令自动生成，**不要手动编辑已生成文件**（如需补充，在下一期报告中体现）。

### 2a. 日报 `daily/YYYY-MM-DD.md`

**命令：** `/market-daily [--date YYYY-MM-DD]`

每个交易日收盘后生成。包含：
- 市场情绪（Fear & Greed）
- 主要指数（SPY / QQQ / DIA / IWM）
- 板块表现（涨跌前三）
- Watchlist 个股（含量比）
- 期权流 / 暗池大单（来自 unusual_whales bot）
- 今日要闻
- AI 解读（市场概况、板块轮动、Watchlist 亮点、社交情绪）
- 今日潜力股候选（T/S/O/F 四维度评分）
- **赛道健康度 · ETF 信号**（四大赛道 Chen Yun 密度 + ETF vs MA50 + F&G，出现 🔴 时运行 `/sector-check`）

周末日报格式简化（无行情数据，只有要闻 + 社交情绪）。

**索引：** `outputs/market/index.md` 自动维护最近 30 条日报的摘要行。

### 2b. 周报 `weekly/YYYY-Www.md`

**命令：** `/market-weekly`

每周五收盘后生成。回顾本周行情、Watchlist 周表现、Chen Yun 观点周盘点。

**命名示例：** `2026-W18.md`（ISO 周编号）

### 2c. 月报 `monthly/YYYY-MM.md`

**命令：** `/market-monthly [--month YYYY-MM]`

每月末生成。包含：
- 主要指数月表现
- Watchlist 月度表现（含论文对齐状态）
- 今日潜力股候选月度胜率统计
- 陈云观点月度复盘（命中率、最佳/最差押注）
- AI 解读（bullet 格式）
- 下月展望（技术面、关键宏观日历、Watchlist 催化剂）

### 2d. 季报 `quarterly/YYYY-Qn.md`

**命令：** `/market-quarterly`

每季末生成。基于三个月报的聚合回顾 + 下季展望。

---

## 3. kb-sync 如何处理 outputs/

运行 `/kb-sync`（即 `py scripts/build_stock_kb.py`）时：

1. **清空** `stock-kb/outputs/`
2. **复制 upstream** `rwh/outputs/` → `stock-kb/outputs/`，并注入 `source: upstream` frontmatter
3. **叠加 overlay** `rwh-overlay/outputs/` → `stock-kb/outputs/`，overlay 文件**不覆盖同名 upstream 文件**，并注入 `source: austin` frontmatter

合并后，`stock-kb/outputs/` 同时包含 upstream 初始分析和 Austin 扩展，可通过 `source` 字段区分。

---

## 4. 使用规则

| 场景 | 操作 |
|------|------|
| 查看某 ticker 所有历史分析 | `ls outputs/<TICKER>/` |
| 新增入场计划 | `/stock-entry <TICKER>`（自动写入 `outputs/<TICKER>/`）|
| 生成今日市场报告 | `/market-daily`（自动写入 `outputs/market/daily/`）|
| 翻查历史日报 | 查 `outputs/market/index.md` 找日期，点链接 |
| 同步到 stock-kb | `/kb-sync` |
| **不要做的事** | 手动编辑已生成的快照文件；upstream 文件由 kb-sync 管理 |
