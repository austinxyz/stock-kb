---
source: austin
---

# UBER — Changelog

Per-ticker change log documenting thesis evolution and action triggers.
**Language**: English | [中文](changelog.zh.md)

---

## 2026-08-06 — Q2 2026：运营超预期，Q3 指引落空，加仓触发未通过 (via /stock-refresh)

Q2 2026（2026-08-05 发布）**运营端交出了论点最想看到的东西**：总订单额 **$58.0B（+24% YoY / +22% cc）** 超共识 $57.23B、落在指引 $57.5–59.5B 区间上半部；**TTM 自由现金流首次突破 $100 亿**；行程 39 亿次（+18%）；月活 2.08 亿（+16%）。营收 $14.19B（+12%）**略低于共识 $14.262B 约 −0.5%**（六季以来首次未超）；Non-GAAP EPS $0.81 vs 共识 $0.805，基本符合（此前五季平均超预期约 +18%，本季实质是「符合」）。

**🔴 但 Q3 指引双双低于共识**：订单额中值 $59.25B vs 共识 $59.33B、Non-GAAP EPS 中值 $0.86 vs $0.89。缺口都很小，方向一致向下，且出现在运营指标全面强劲的同一份财报里 —— 当日 **−5.29%** 至 **$68.18**。

**🔴 上一版明确写下的加仓触发条件被检验且未通过。** 原文：「HOLD，Q2 财报后看 MA50 回收再加仓」。实际价格距 MA50 由 −3.9% 扩大至 **−4.8%**（MA50 $71.99→$71.65），**方向相反**。Stage 4 / Death Cross 维持，距 52 周低点 $65.41 仅 4.2%（7/30 为 5.6%），止损 $63.00 就在该低点下方 3.7%。**不加仓。**

**30 日预期修正四个周期全部反向**：本季 3↑/0↓ → **0↑/2↓**；下季 4↑/0↓ → 1↑/2↓；本年 3↑/1↓ → 1↑/3↓；次年 4↑/0↓ → 2↑/3↓。上一版把「修正方向已回正」称为**「等待期内最积极的信号之一」**，该判断已被指引推翻。**保留原文不改写** —— 教训不是当时读错（当时证据确实支持它），而是**财报前的修正动能只是「对预期的预期」，指引落地当天可整段作废**，不应作为等待期主要依据。

**记录一处口径陷阱：** yfinance 的 UBER EPS surprise 列不可用 —— 它拿 **GAAP 摊薄 EPS** 比 **非 GAAP 共识**，而 Uber 的 GAAP 净利被权益投资按市值重估主导。实证：Q1 2026 营业利润 $1.923B（近四季最高）但 GAAP 净利仅 $0.263B（yfinance 记 −81.7%）；Q3 2025 营业利润 $1.113B 却录得净利 $6.626B（记 +353%）。已写入 financials.md 文件头警告。

**数据来源标注：** yfinance 截至 2026-08-06 未收录 Q2 实际（`mostRecentQuarter` 仍为 2026-03-31）。Q2 数字取自财报报道，**年度三张财务表未改动**，待 10-Q 核对。

**前次论点状态**: Intact（HOLD，等 MA50 回收再加仓）→ **更新后**: **Weakened 未 Broken**（HOLD 不变，**加仓触发已明确失败**，止损维持 $63.00）

---

## 2026-07-30 — 财报倒计时 6 天 + 50 天未刷新 + Stage 4 维持 (via /stock-refresh)

价格 $69.11（今日 -2.98%，vol_ratio **26.62x**；可能 Delivery Hero 消息或 FOMC 后市场反应）。自 6/10 $70.38 小幅下跌 -1.8%，但期间 52 周新低触至 **$65.41**（已部分回升）。MA50 $71.99（价格仍 -3.9% 下方）—— **Stage 4 维持，MA50 回收条件未满足**。估值修正转正：Q2 30d 修正 3↑/0↓（原 DOWN30d=29，大幅改善）；FY2026 3↑/1↓；FY2027 4↑/0↓。FY2026 营收共识 $58.2B（vs overlay 估算 $61.6B，下修 ~5.5%）。**Q2 财报日确认：2026-08-05（6 天后）**。Delivery Hero 收购决定仍未明朗，今日高量或与此相关。
**前次论点状态**: Hold（Stage 4，等 MA50 回收）→ **更新后**: Hold（不变；加仓触发 = 财报后 MA50 $71.99 放量回收）

---

## 2026-06-10 — rwh upstream merge + technical/sentiment refresh (via /stock-analyze)

Merged rwh v3.0 (As-of 2026-05-22) into the overlay + refreshed technicals/sentiment at $70.38 (2026-06-10). Verdict shifted from "Watch, Initiate <$85" to **active-holding stance: HOLD; thesis intact + price inside rwh's $65–80 entry zone, BUT SEPA Stage 4 at the 52-wk low — wait for MA50 ($73.63) reclaim on volume before adding, don't catch the falling knife.** Key changes: (1) PW EV held at $195, but spot down to $70.38 → upside +177%, R/R improved to ~11–12:1; (2) NEW May-2026 capital-allocation escalation — $10B+ AV commitments (Lucid/Nuro, Rivian, Wayve/Avride/Baidu) + Delivery Hero stake→25.1% with full takeover under study — added as the dominant new bear prong, two new §8 risks, two new thesis-break triggers, and an Outsider-grade caveat (Outsider-leaning → Reinvestor if AV/DH crowds out buyback); (3) technical degraded from "Stage 1 basing, 1/8" to **Stage 4 / downtrend at 52-wk low, below all MAs, ~1–2/8**; (4) near-term estimates being CUT (0y revisions DOWN30d=29) but +1y EPS $4.46 (+51%) intact; (5) sentiment Mildly Bullish / high-attention (Adanos 7d: X+news bullish, Reddit neutral-bearish). BAIT T-lens dropped MODERATE→WEAK.

## 2026-05-08 — Initial Analysis (via /stock-analyze)

Q1 2026 beat day ($75.45, +5.93%): PW EV $195 (R/R 9.4:1 vs entry <$85); SEPA 1/8 → Watch; moat Wide; upstream Initiate <$85; full 15-section thesis written.
