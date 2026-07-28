---
source: austin
---

# KWEB — Changelog

In reverse chronological order.

---

## 2026-07-28 — Full Refresh (via /etf-analyze)

Price $27.29. **Verdict upgraded Avoid → Watch** on the MA50 reclaim named as the upgrade condition in the May analysis. Trend template 0/8 → **1/8** — the single passing criterion is price > MA50 ($26.37, +3.5%).

The upgrade is deliberately capped at Watch, not Use, because the reclaim is half-proven on three counts:
- **2 of 3 required sessions**, volume ratios 0.88× / 0.38× — no volume confirmation. A prior attempt held above MA50 for 5 sessions from 7/15 before failing 7/22.
- **The MA50 descended to the price, not the reverse.** On 2026-06-03 MA50 was $28.56; today $26.37. Price $27.29 is still below where the MA50 sat in June.
- **PW EV +7.7%** (Bull $36 25% / Base $30 45% / Bear $23 30%) trails SPY's trailing-year +17.7%.

**Two data-integrity corrections:**
1. **NAV premium/discount is unusable from yfinance for this fund family.** All four China ETFs printed a same-signed premium of comparable magnitude on 2026-07-28 (KWEB +2.74%, CQQQ +2.02%, FXI +1.85%, MCHI +1.74%) — a market-hours mismatch artifact, not fund-specific pricing. The "−2.15% NAV discount" recorded on 2026-05-22 and propagated into `etf-reference.md` was most likely the same artifact on a down day. Both references removed.
2. **AUM fell $6.35B → $4.91B (−22.7%) in two months on a flat price** ($26.89 → $27.29) — redemption-driven, not mark-to-market. 30d volume 31.32M → 21.24M shares. Added as the top-probability risk.

**Trigger-design flaw logged as S007**: the 2026-06-03 upgrade condition "reclaim MA50 **$28.87** on volume 3 days" hard-codes a dollar value for a moving average. Both the dynamic and fixed readings return "not met" today so there is no conflict to resolve, but the ambiguity is the same defect class as S002.

Purity unchanged at High (~96%), liquidity grade A. Peer note: CQQQ returned +8.1% over 1 year vs KWEB −19.6% — what outperformed in China was hardware, not internet platforms.

---

## 2026-06-03 — Exit Analysis

**Category:** B thematic/conviction | **Decision:** trim/exit OR conviction Hold — user's call
**Exit trigger:** broke MA50 $28.56 + thesis Avoid + Stage 4 (all three MAs overhead)
**File:** [exit-2026-06-03.md](../../../data/outputs/etf/KWEB/exit-2026-06-03.md) *(private — gitignored)*

---

## 2026-05-22 — Initial Analysis (via /etf-analyze)

Price $26.89, testing 52-week low $26.41 on vol ratio 114× (FUTU/TIGR −37%/−34% China selloff). SEPA 0/8, Stage 4 full downtrend. Verdict: **Avoid**. Highest-purity China internet ETF but all MAs above price; p-weighted EV only +4.2% including 7.42% yield. Upgrade condition: MA50 ($28.87) reclaim on volume.

> ⚠️ *Superseded 2026-07-28*: this entry also recorded a "NAV discount −2.15%", now identified as a data artifact rather than a fund characteristic. See the 2026-07-28 entry.
