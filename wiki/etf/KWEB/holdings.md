---
source: austin
---

# KWEB — Holdings & Composition

**Last updated**: 2026-07-28
**Data source**: yfinance / KraneShares as of 2026-07-28
**Next update trigger**: Semi-annual index rebalance, or any single holding crossing the 10% cap
**Language**: English | [中文](holdings.zh.md)

## Top Holdings

| # | Ticker | Company | Weight % | On-theme? |
|---|--------|---------|----------|-----------|
| 1 | 0700.HK | Tencent Holdings Ltd | 10.46% | ✅ core platform |
| 2 | PDD | PDD Holdings Inc ADR | 7.93% | ✅ e-commerce |
| 3 | 9988.HK | Alibaba Group Holding | 7.71% | ✅ e-commerce / cloud |
| 4 | 9999.HK | NetEase Inc | 6.98% | ✅ gaming |
| 5 | 3690.HK | Meituan Class B | 6.84% | ✅ local services |
| 6 | 9888.HK | Baidu Inc | 4.20% | ✅ search / AI |
| 7 | YMM | Full Truck Alliance Co ADR | 4.16% | ✅ logistics platform |
| 8 | 1024.HK | Kuaishou Technology Class B | 4.08% | ✅ short video |
| 9 | 2423.HK | KE Holdings Inc Class A | 3.90% | ⚠️ property brokerage |
| 10 | 9618.HK | JD.com Inc Class A | 3.88% | ✅ e-commerce |

*yfinance exposes only the top 10. Full holdings list: KraneShares fund page.*

**Concentration**: Top 5 = 39.9% · Top 10 = 60.1%

Tencent at 10.46% is the only position above 10% and sits at the index single-issuer cap. No runaway concentration, but a Tencent-specific shock transmits directly.

## Sector Weights

| Sector | Weight % |
|--------|----------|
| Communication Services | 46.2% |
| Consumer Cyclical | 34.0% |
| Healthcare | 5.8% |
| Technology | 4.2% |
| Consumer Defensive | 4.0% |
| Real Estate | 3.9% |
| Financial Services | 1.9% |
| Basic Materials / Utilities / Industrials / Energy | 0.0% |

Note the shape: 80.2% of the fund sits in just two GICS buckets. The "Technology" line reading only 4.2% is a classification artifact — Chinese platform companies are classified as Communication Services or Consumer Cyclical, not Technology.

## Asset Classes

| Class | Weight % |
|-------|----------|
| Stock | 99.9% |
| Cash | 0.1% |
| Bond / Preferred / Convertible / Other | 0.0% |

Fully invested, no derivative overlay.

## Geographic Exposure

Effectively 100% China by revenue source. Listing venues split between Hong Kong (H-shares) and US ADRs. No mainland A-share exposure by index design.

This offshore-listing screen is the single most important structural fact about the fund: it defines both the opportunity (ADR/H-share valuation discount) and the tail risk (US-China listing policy, VIE structure).

## Index Methodology

**CSI Overseas China Internet Index** — market-cap weighted, capped at 10% per issuer, rebalanced semi-annually. Selection requires: China-based operations, internet or internet-adjacent business model, listing outside mainland China, and a liquidity screen.

Rebalance risk is modest for a fund this concentrated — the top names are stable across cycles. The cap mechanism forces a trim of Tencent at each rebalance whenever it drifts above 10%.

## Tracking Quality

| Metric | Value |
|--------|-------|
| Expense ratio | 0.76% |
| Tracking difference (1y) | not available |
| Tracking error (annualized) | not available |
| NAV premium/discount | **unusable — see note** |
| Benchmark index | CSI Overseas China Internet Index |

### Note — NAV premium/discount cannot be measured from yfinance

On 2026-07-28 yfinance implies a +3.84% premium (price $27.29 vs NAV $26.28). This is rejected as an artifact.

Cross-check on the same date across the China ETF peer set:

| Ticker | Prev close | yfinance NAV | Implied "premium" |
|--------|-----------|--------------|-------------------|
| KWEB | $27.00 | $26.28 | +2.74% |
| CQQQ | $51.09 | $50.08 | +2.02% |
| FXI | $35.28 | $34.64 | +1.85% |
| MCHI | $54.26 | $53.33 | +1.74% |

Four unrelated funds showing a same-signed premium of comparable magnitude on the same day indicates a **systematic market-hours mismatch**, not fund-specific pricing. HK and A-share markets close hours before the US session; NAV is struck against stale underlying prices.

The 2026-05-22 analysis recorded "−2.15% NAV discount" as a KWEB characteristic. That was most likely the identical artifact observed on a down day, and it propagated into `etf-reference.md`. Both have been removed. Genuine premium/discount and tracking-difference figures require the issuer's published daily NAV series.

## Fund Flows

| Date | AUM | Change |
|------|-----|--------|
| 2026-05-22 | $6.35B | — |
| 2026-07-28 | $4.91B | **−22.7%** |

Over the same window price moved from $26.89 to $27.29 — roughly flat. The AUM decline is therefore redemption-driven, not mark-to-market. 30-day average volume also fell from 31.32M to 21.24M shares.

This is the fund-level metric worth watching most closely. Below $3B AUM, spread and tracking quality begin to degrade materially.

## Upcoming Rebalances

| Date | Event | Expected Impact |
|------|-------|----------------|
| Semi-annual (next date TBC) | Index reconstitution + 10% cap reset | Low — top names stable; Tencent trimmed back toward cap if above |
