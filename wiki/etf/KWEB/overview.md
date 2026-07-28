---
source: austin
---

# KWEB — KraneShares CSI China Internet ETF

**Last updated**: 2026-07-28
**Status**: Watch — reclaimed MA50 but only 2 sessions and without volume; trend template 1/8
**Sector**: 中国互联网 / China Internet
**Language**: English | [中文](overview.zh.md)

## ETF at a Glance

| Field | Value |
|-------|-------|
| Full name | KraneShares CSI China Internet ETF |
| Fund family | KraneShares (Krane Funds Advisors) |
| Index tracked | CSI Overseas China Internet Index (passive) |
| Inception | 2013-07-31 |
| AUM | $4.91B (was $6.35B on 2026-05-22 — **−22.7% in 2 months**) |
| Expense ratio | 0.76% |
| Distribution yield | 8.61% (⚠️ return-of-capital component unverified) |
| 30d avg volume | 21.24M shares (~$580M/day) |
| YTD return | −28.96% |

## Sector Purity

**High (~96%)** — 10 of 10 top holdings are core China internet / platform names. Only dilution is KE Holdings (3.9%), a property-transaction platform that carries China real-estate cycle exposure.

No peer competes on purity: FXI holds state-owned financials, MCHI is broad-market, CQQQ includes hardware.

Top holdings aligned to theme: 10 of 10

## Technical Summary

| Metric | Value |
|--------|-------|
| Price | $27.29 |
| 50MA | $26.37 (+3.5%) |
| 150MA | $29.95 (−8.9%) |
| 200MA | $31.55 (−13.5%) |
| 52-wk range | $23.23 – $40.87 |
| Distance from 52-wk high | −33.2% |
| Distance from 52-wk low | +17.5% |
| ATR(14) | $0.39 |
| Stage | 4 → early 1 (base attempt) |
| Trend template | **1/8** (was 0/8) |
| Pattern | none — first base attempt off the low |
| SEPA verdict | Watch |

**The only passing criterion is price > MA50.** MA50 sits below both MA150 and MA200 and all three slope down.

**Critical framing**: the MA50 came *down* to the price, not the other way round. On 2026-06-03 MA50 was $28.56; today it is $26.37. Price $27.29 is still **below** the June MA50 level.

Consecutive closes above MA50: **2** (7/27, 7/28). Volume ratios 0.88× / 0.38× — **no volume confirmation**. A prior attempt on 7/15–7/21 held above MA50 for 5 sessions before failing on 7/22.

## Peer Comparison (Quick)

| Ticker | Expense Ratio | 30d Vol | AUM | 1y Return | Verdict |
|--------|--------------|---------|-----|-----------|---------|
| **KWEB** | 0.76% | 21.2M | $4.91B | −19.6% | Purest + most liquid; worst performer |
| CQQQ | 0.70% | 1.3M | $3.42B | **+8.1%** | Only positive 1y; 16× less liquid |
| FXI | 0.74% | 25.6M | $4.52B | −5.6% | Broad large-cap, state financials |
| MCHI | 0.59% | 3.1M | $5.89B | — | Cheapest, least pure |

## DCA Trigger Conditions

Accumulation zone: **$25.6–$27.2** (MA50 ±3%). Price has just exited the upper edge.
MA200 $31.55 sits *above* price — the deep-discount zone does not apply this cycle.

Upgrade to **Use** requires all three:
1. 3 consecutive closes above MA50 **with** at least one session at ≥1.5× volume
2. MA50 slope turns up (currently still declining)
3. AUM stabilizes (stop the −22.7% bleed)

Downgrade to **Avoid**: close below $25.6 (MA50 −3%), or AUM below $3B.

## Data Quality Note — NAV Premium Unusable

yfinance reports price $27.29 vs NAV $26.28 = +3.84% premium. **This figure is an artifact, not a real premium.**

All four China ETFs show a same-signed premium of similar magnitude on the same day (FXI +1.85%, MCHI +1.74%, CQQQ +2.02%) — a systematic bias consistent with **market-hours mismatch**: HK/A-share markets close hours before the US session, so NAV is struck against stale underlying prices.

**Implication**: the "−2.15% NAV discount" recorded in the 2026-05-22 analysis was most likely the same artifact read on a down day, and was propagated into `etf-reference.md` as a KWEB characteristic. Both have been removed. Genuine premium/discount requires the issuer's daily NAV disclosure; yfinance cannot supply it for this fund family.

## Why It's In The Wiki

Added 2026-05-22 as the purest available vehicle for the China-internet mean-reversion thesis. Chosen over CQQQ/FXI/MCHI on purity and liquidity. See [thesis.md](thesis.md).
