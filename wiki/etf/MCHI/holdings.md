---
source: austin
---

# MCHI — Holdings & Composition

**Last updated**: 2026-08-11
**Data source**: Yahoo Finance (yfinance `fetch_ticker.py`) as of 2026-08-11
**Next update trigger**: MSCI semi-annual index rebalance (~May/November) or major holding change
**Language**: English | [中文](holdings.zh.md)

## Top Holdings

| # | Ticker | Company | Weight % | On-theme? |
|---|--------|---------|----------|-----------|
| 1 | 0700.HK | Tencent Holdings Ltd | 14.5% | ✅ |
| 2 | 9988.HK | Alibaba Group Holding | 9.7% | ✅ |
| 3 | 00939 | China Construction Bank Corp Class H | 3.8% | ❌ |
| 4 | 1810.HK | Xiaomi Corp Class B | 2.4% | ⚠️ |
| 5 | 01398 | Industrial And Commercial Bank Of China Class H | 2.4% | ❌ |
| 6 | 3690.HK | Meituan Class B | 2.3% | ✅ |
| 7 | PDD | PDD Holdings Inc ADR | 2.0% | ✅ |
| 8 | 02318 | Ping An Insurance (Group) Class H | 1.9% | ❌ |
| 9 | 03988 | Bank Of China Ltd Class H | 1.8% | ❌ |
| 10 | 9999.HK | NetEase Inc | 1.8% | ✅ |

*Only top 10 available from the current data pull; full constituent list not fetched in this pass.*

## Sector Weights

| Sector | Weight % |
|--------|----------|
| Consumer Cyclical | 25.0% |
| Financial Services | 19.8% |
| Communication Services | 19.4% |
| Technology | 10.6% |
| Healthcare | 5.3% |
| Basic Materials | 5.2% |
| Industrials | 5.0% |
| Energy | 3.5% |
| Consumer Defensive | 3.1% |
| Utilities | 1.6% |
| Real Estate | 1.5% |

## Asset Class Breakdown

| Class | Weight % |
|-------|----------|
| Stocks | 99.1% |
| Cash | 0.9% |
| Bonds/Preferred/Convertible | 0.0% |

## Index Methodology

MCHI tracks the MSCI China Index — market-cap-weighted, covering large- and mid-cap Chinese equities accessible to international investors (H-shares, B-shares, Red-chips, P-chips, and relevant US-listed ADRs). MSCI rebalances the index semi-annually (typically May and November) per standard MSCI Global Investable Market Index methodology. Full index methodology document not independently reviewed in this pass.

## Tracking Quality

| Metric | Value |
|--------|-------|
| Expense ratio | 0.59% |
| Current NAV premium/discount | -1.85% (price $55.72 vs. NAV $56.7684, 2026-08-11 snapshot) |
| Tracking difference (1y) | Not independently computed this pass |
| Tracking error (annualized) | Not independently computed this pass |
| Benchmark index | MSCI China Index |

**Note on the -1.85% NAV discount**: `wiki/etf/etf-reference.md` documents that same-day premium/discount readings for China-market ETFs during US trading hours are frequently distorted by the HK/China market closing well before the US session — a timezone-mismatch artifact rather than a genuine pricing dislocation. This reading should not be treated as a real, exploitable discount without cross-checking against a same-timezone NAV snapshot.

## Upcoming Rebalances

| Date | Event | Expected Impact |
|------|-------|------------------|
| ~November 2026 | MSCI semi-annual rebalance | Standard index reconstitution; watch for any material sector-weight shift toward/away from internet names |
