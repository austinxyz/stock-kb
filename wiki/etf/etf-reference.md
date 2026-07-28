---
source: austin
---

# ETF 赛道参考表

*手动维护。每季度或新 ETF 上市时更新。*
*费率来源：ETF 官网/SEC filing。流动性 = 30日均量（百万股）。*

## 电网 + 储能 / Grid

| Ticker | 名称 | 费率 | 30日均量 | 说明 |
|--------|------|------|---------|------|
| GRID | First Trust NASDAQ Clean Edge Smart Grid & Infrastructure | 0.70% | 0.750M | 最纯电网 ETF；AUM $7.65B；[详细分析](GRID/overview.md) |
| ICLN | iShares Global Clean Energy | 0.41% | 6.27M | 流动性最好，但含风光等非电网 |
| TAN | Invesco Solar | 0.69% | 1.19M | 纯光伏，赛道主题较窄 |
| QCLN | First Trust NASDAQ Clean Edge Green Energy | 0.59% | 0.14M | 较平衡，含 EV；流动性偏低 |

**当前推荐：GRID**（最贴合赛道主题，AUM $7.65B 充足；注：前十持仓中无直接SiC/储能标的，SiC层由个股WOLF/EOSE覆盖）

## 存储芯片 / AI Memory

| Ticker | 名称 | 费率 | 30日均量 | 说明 |
|--------|------|------|---------|------|
| SOXX | iShares Semiconductor | 0.35% | 6.81M | 最大半导体 ETF，含 AI Memory；AUM $205.9亿；[详细分析](SOXX/overview.md) |
| SMH | VanEck Semiconductor | 0.35% | 8.56M | 流动性最高，NVDA 权重大；AUM $41B |
| DRAM | Roundhill Memory ETF | ~0.59% | 9.4M | 🆕 2026-04-02 上市；纯 DRAM/HBM 主题（MU/SK Hynix/WDC）；AUM 待确认；⚠️ 上市仅 22 天，无 MA50；触发后可替代 SOXX 作为更聚焦工具；⚠️ NVTS（Navitas/GaN）疑为参考表数据错误，待官方持仓确认；[详细分析](DRAM/overview.zh.md) |

**当前推荐：SOXX**（比 SMH 更分散，不过度集中 NVDA；比 DRAM 有更长流动性记录）
**备选关注：DRAM**（HBM/AI Memory 更纯净主题；等有效历史建立后评估；理想入场区 $35–38）

## 光互连 / Optical Interconnect

| Ticker | 名称 | 费率 | 说明 |
|--------|------|------|------|
| — | 无纯光互连 ETF | — | 以 NVTS+COHR 个股篮子替代（POET 已于 2026-05-08 放弃）|

**篮子 MA50 计算方式（替代 ETF vs MA50）：**

赛道健康度表中的"ETF vs MA50"栏，对无 ETF 赛道使用**个股市值加权均值**：

```
篮子 MA50 偏离 = Σ (个股当前市值权重 × 个股 vs MA50%)
```

计算工具：
```bash
python scripts/morning_scan.py --basket NVTS:50 COHR:3 --json
# 输出: {"ticker": "NVTS+COHR", "basket": true, "ma50_pct": 46.7, "components": [...]}

python scripts/morning_scan.py --basket NVTS:50 COHR:3
# 输出: NVTS+COHR  basket  ma50_pct=+46.7%  total=$2,213  (NVTS 48% +66.6%, COHR 52% +28.3%)
```

触发规则与 ETF 完全相同：
- 路径A：篮子均值 ≤ −5% → 触发（恐慌买入信号）
- 路径B：篮子均值 > 0% → 通过（上行趋势确认）

篮子构成变动时，更新 `--basket` 中的 TICKER:SHARES 参数。

## 低轨卫星 / LEO

| Ticker | 名称 | 费率 | 30日均量 | 说明 |
|--------|------|------|---------|------|
| UFO | Procure Space ETF | 0.75% | 1.01M | 🆕 2026-05-16 加入；追踪 S-Network Space Index；太空经济全产业链（卫星通信/发射/地球观测/GPS）；AUM $7.49 亿；NAV 溢价 +0.065%（极低）；[详细分析](UFO/overview.md) |
| ARKX | ARK Space Exploration & Innovation | 0.75% | 0.78M | 主动管理，含防务/无人机；AUM $8.93 亿 |
| ROKT | SPDR S&P Kensho Final Frontiers | 0.45% | 0.04M | 流动性极差（0.04M/日），实际不可用 |

**当前推荐：UFO**（流动性优于 ARKX +30%，近期 alpha 大幅领先：6M +68.7% vs +22.4%，费率相同；Wait 评级，等 SPCX IPO 后回调至 $49–$53（MA50 ± 3%）入场；现价 $61.41 不追）
**备选：ARKX**（历史更长，AUM 略大）
**排除：ROKT**（流动性不足）

## 半导体封装 / Advanced Packaging

*🆕 2026-05-26 新增赛道（Chen Yun 新瓶颈论：电力 + 半导体封装）。*

| Ticker | 名称 | 费率 | 30日均量 | 说明 |
|--------|------|------|---------|------|
| — | 无纯封装 ETF | — | 市场无纯先进封装/封测主题 ETF；SOXX/SMH 半导体宽基有部分重叠但非聚焦 |
| SOXX | iShares Semiconductor | 0.35% | 6.81M | 含 AMKR/封测成分，但稀释于宽半导体；与存储芯片赛道共用 |
| SMH | VanEck Semiconductor | 0.35% | 8.56M | 同上，TSM 权重较大 |

**代表个股（Chen 点名 TSM / ASX / GFS / AMKR）：**

| Ticker | 角色 | 备注 |
|--------|------|------|
| TSM | 台积电 — CoWoS 先进封装龙头 | ADR；AI 封装产能瓶颈核心受益者 |
| ASX | 日月光 — 全球最大 OSAT 封测厂 | ADR；外包封测龙头 |
| AMKR | Amkor — 美国本土封测纯标的 | 美国制造回归 + 政府补贴 4 亿美元；唯一美国本土纯封测标的 |
| GFS | 格芯 — 代工厂（非纯封装）| ⚠️ Chen 归为封装，实为晶圆代工；在美扩建高端封装厂 |

**当前推荐：暂缓 ETF 化**
- 无纯封装 ETF → 该赛道仅能用个股篮子表达，或暂用 SOXX 间接覆盖
- 若建仓，AMKR 为最纯美国本土封测标的；TSM/ASX 为 ADR 龙头
- ⚠️ 篮子 MA50 计算方式同光互连（个股市值加权），等实际建仓后用 `--basket` 工具

## AI 企业软件 / AI Enterprise Software

*🆕 2026-06-01 新增赛道（sector-analyze）。赛道论文：[wiki/sectors/ai-enterprise-software.md](../sectors/ai-enterprise-software.md)。可投性 Watch（近 Go）· 生命周期 成熟。*

| Ticker | 名称 | 费率 | 30日均量 | 说明 |
|--------|------|------|---------|------|
| IGV | iShares Expanded Tech-Software | ~0.41% | 高 | ✅ 推荐打底（最纯应用软件；持仓 CRM/NOW/ADBE/INTU/PANW 等）|
| WCLD | WisdomTree Cloud Computing | 0.45% | 中 | 纯云/SaaS，但偏中小盘、波动大 |
| PInG / SKYY | 云计算宽基 | 0.60%/0.68% | 中 | 含基建/超大盘云（含 AMZN/MSFT/GOOG），非纯应用软件 |

**代表卫星个股（赛道论文 §10）：**

| Ticker | 角色 | 备注 |
|--------|------|------|
| INTU | 深度价值卫星 | Intuit；等 Q4 FY26 财报(8/20) Stage 2 确认 |
| CRM | 大盘锚 | Salesforce；AI Agentforce 试金石 |
| FIG | 逆境股卫星 | Figma；设计协作层，等重回 MA200 |

**当前推荐：IGV 打底（等回调）**
- IGV = 最纯应用软件 ETF，赛道论文选定打底载体
- ⚠️ 截至 2026-06-03：IGV $100.81，价 +15.8% 高于 MA50 $87.08，但 MA50<MA150<MA200 未黄金交叉（非干净 Stage 2）；等回踩 MA150/MA200 区 $94–99 或 §9 升 Go
- ⚠️ 该赛道尚未配置 positions.py DCA 目标（仅 4 赛道：电网/存储/光互连/LEO）；升 Go 决定打底后再配目标
- **升级触发：** IGV 站稳 MA50 + 高量突破且 MA 黄金交叉，或 INTU/CRM Stage 2 技术确认 → §9 升 Go

## 中国互联网 / China Internet

| Ticker | 名称 | 费率 | 30日均量 | 说明 |
|--------|------|------|---------|------|
*数据截至 2026-07-28。*

| Ticker | 名称 | 费率 | 30日均量 | AUM | 1年 | 说明 |
|--------|------|------|---------|-----|-----|------|
| KWEB | KraneShares CSI China Internet ETF | 0.76% | 21.24M | $4.91B | −19.6% | 中国互联网纯度最高（约96%）；流动性最强（约$580M/日）；⚠️ AUM 2个月 −22.7%；[详细分析](KWEB/overview.zh.md) |
| CQQQ | Invesco China Technology ETF | 0.70% | 1.32M | $3.42B | **+8.1%** | 中国科技（含硬件）；唯一 1 年正收益的中国 ETF；流动性差 16× |
| FXI | iShares China Large-Cap ETF | 0.74% | 25.60M | $4.52B | −5.6% | 宽基大盘，含大量国有金融股；纯度低 |
| MCHI | iShares MSCI China ETF | 0.59% | 3.10M | $5.89B | — | 最宽基中国市场；纯度低；流动性低 |

> ⚠️ **NAV 溢价/折价数据对该组不可用。** yfinance 同日给出四只同向、同量级溢价
> （KWEB +2.74%、CQQQ +2.02%、FXI +1.85%、MCHI +1.74%）—— 港股/A 股收盘早于美股的
> **时段错配伪影**，非基金特有定价。本表此前记录的 KWEB「NAV 折价 −2.15%」（2026-05-22）
> 大概率是同一伪影在下跌日的读数，已删除。真实溢价需发行商每日 NAV 披露。

**当前推荐：KWEB — Watch（2026-07-28 自 Avoid 升级）；其余 Avoid**
- KWEB：收复 MA50（$26.37，+3.5%），趋势模板 0/8 → **1/8**。但仅 2/3 个交易日且无量能确认，且 **MA50 是降下来接住价格的**（6/3 时 MA50 $28.56，今 $26.37）→ 只升 Watch 不升 Use
- CQQQ：1 年 +8.1% 为组内唯一正收益，但流动性仅 1.32M/日；且它表达的是「中国科技硬件」而非「中国互联网平台」，论点不同
- FXI/MCHI：宽基，不代表纯中国互联网论点

**升级触发（2026-07-28 修正措辞）：** KWEB 连续 3 日收于**当时的** MA50 上方，其中至少一日量比 ≥1.5×，且 MA50 斜率非负 → 升 Use。
> 原措辞为「收复 MA50 **$28.87** 放量 3 日」，把移动均线硬编码成固定美元值（S007，同 S002 缺陷类别）。

**降级触发：** KWEB 收盘跌破 $25.6（MA50 −3%），或 AUM 跌破 $3B（当前 $4.91B，2 个月已失血 22.7%）
