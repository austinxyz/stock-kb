---
source: austin
---

# NVTS — Full Investment Thesis

**Ticker**: NVTS (Nasdaq)
**Company**: Navitas Semiconductor Corporation
**As of**: 2026-07-10
**Price**: $13.47 (–5.01% today, vol_ratio 35.77×)
**52-wk range**: $1.80 – ~$29.25 (May 22 peak)
**Market cap**: ~$3.28B
**Verdict**: **Speculative — Watch; Stage 3 correction; no position; Q2 earnings Jul 27 is the binary; base case already priced in at current level**
**Language**: English | [中文](thesis.zh.md)

---

## 1. Why Does This Company Exist? + Pivotal Investment Question

**Raison d'être**: Navitas designs wide-bandgap (WBG) power semiconductors —
GaN and SiC — that switch faster and handle higher voltages than traditional
silicon MOSFETs. In power electronics (AC/DC conversion, motor drives,
inverters), WBG reduces losses, shrinks system size, and enables new
architectures like NVIDIA's 800V HVDC rack power.

**Strategic transition (FY2025)**: The company deprioritized low-margin China
mobile-charger business (previously majority of revenue) to focus on four
high-power markets: **AI datacenter, grid/energy infrastructure, high-
performance computing, and industrial electrification**. Q4 2025 was the
first quarter in company history where high-power markets were >50% of
revenue; mobile is now <25%.

**Pivotal Question**: *Can execution on the NVIDIA partnership + GlobalFoundries
GaN manufacturing partnership produce a real, profitable high-power revenue
base before cash runway or competitive displacement forces another capital
raise?*

Answer depends on 4 variables: (1) pace of 800V HVDC architecture adoption
by hyperscalers, (2) Navitas's share of NVIDIA's multi-sourced power BOM,
(3) SiC price decline trajectory (WOLF, STM, ON all expanding capacity),
(4) how the Q2-Q4 2026 revenue ramp actually materializes vs. current
guidance ($8–8.5M for Q1, implying low double-digit million quarters into
H2 2026).

---

## 2. Annual Financial Metrics

### Income Statement (FY2021–FY2025)

| $ millions | FY2021 | FY2022 | FY2023 | FY2024 | FY2025 |
|------------|-------:|-------:|-------:|-------:|-------:|
| Revenue | 23.7 | 37.9 | 79.5 | 83.3 | **45.9** |
| Gross Profit | 10.7 | 11.9 | 31.1 | 28.3 | 14.3 |
| Gross Margin % | 45.0% | 31.5% | 39.1% | 34.0% | 31.0% |
| Operating Loss | –68.5 | –123.6 | –118.1 | –130.7 | **–107.8** |
| Operating Margin | –289% | –326% | –149% | –157% | **–235%** |
| Net Income | –152.7 | +73.9¹ | –145.4 | –80.7 | –118.1 |
| Diluted EPS | –$3.90 | +$0.51 | –$0.86 | –$0.46 | **–$0.57** |
| Diluted Shares (M) | 39 | 146 | 169 | 182 | **206** |

¹FY2022 net income positive due to non-cash warrant revaluation gain, not operating profit.

### Cash Flow

| $ millions | FY2021 | FY2022 | FY2023 | FY2024 | FY2025 |
|------------|-------:|-------:|-------:|-------:|-------:|
| Operating CF | –41.7 | –44.5 | –41.4 | –58.8 | –42.9 |
| CapEx | –2.1 | –4.6 | –4.8 | –6.8 | –1.5 |
| **Free Cash Flow** | **–43.8** | **–49.1** | **–46.2** | **–65.6** | **–44.4** |
| Stock-Based Comp | 41.4 | 63.3 | 54.0 | 43.0 | **14.5** |

### Balance Sheet (FY2025 year-end)

| Metric | Value | Comment |
|--------|------:|---------|
| Cash + Short-term Investments | $237M | Replenished from $87M (FY24) via equity raise |
| Total Debt | $6.5M | Effectively debt-free |
| Total Equity | $444M | |
| Accumulated Deficit | –$502M | Never cumulatively profitable |
| Shares Outstanding | 206M | Up from 39M in FY21 (5.3× dilution) |

### Recent Quarterly Detail

| Quarter | Revenue | QoQ | GM% (non-GAAP) | Notes |
|---------|--------:|----:|---------------:|-------|
| Q4 2024 | $18.0M | — | — | Mobile-heavy era peak |
| Q1 2025 | ~$14M | –22% | — | Mobile decline accelerating |
| Q2 2025 | ~$14M | 0% | — | Continued weakness |
| Q3 2025 | ~$10M | –29% | — | Pivot mid-flight |
| **Q4 2025 (trough)** | **$7.3M** | **–27%** | **38.7%** | **"This is the bottom"** |
| **Q1 2026 (actual)** | **$8.6M** ✅ | **+18%** | **39.0%** | **Beat guidance; EPS –$0.04 vs –$0.05 est** |
| Q2 2026 (guide) | $10.0M ±0.5M | +16% | 39.25% ±75bps | Sequential acceleration confirmed |

---

## 3. Geographic Revenue Mix

Historically skewed Asia (China mobile). Post-pivot mix is migrating toward
US / Europe high-power customers but precise geographic breakdown for FY2025
not disclosed at this detail in press releases reviewed. **[Data gap: 10-K
detail pending]**.

---

## 4. Revenue Mix & Business Model

### Product Lines

| Product | Technology | End Market |
|---------|-----------|-----------|
| GaNFast™ | Monolithic GaN power ICs | Mobile chargers (legacy), EV OBC, datacenter PSUs |
| GeneSiC™ | SiC MOSFETs/diodes (2022 acquisition) | Solar inverters, EV traction, industrial |
| Integrated modules | GaN+SiC co-packaged | AI datacenter 800V HVDC (new) |

### Revenue by Segment (FY2025, mgmt commentary — not precise)

- **Mobile & consumer**: <25% (declining, will be ~10% by FY26)
- **High-power (AI DC / grid / industrial / EV)**: >50% and growing
- **Solar / renewables**: Material but not broken out
- **Automotive (OBC, traction)**: Small but design-win pipeline

**Business model caveats:**
- Fabless (TSMC for GaN → GlobalFoundries US partnership late 2026 → 2027)
- Revenue recognition on design-wins: 12–24 month cycle from win to shipment
- NVIDIA 800V HVDC revenue contribution **not yet in any quarter** — design
  phase today, volume 2027–2028

---

## 5. Competitive Moat

### What Navitas has

- **Monolithic GaN IP**: Drive + control + protection integrated on single die
  (most competitors offer discrete GaN FETs)
- **SiC portfolio via GeneSiC** — broader product line than GaN-only peers
- **NVIDIA "Power Selector Partner" designation** — real ecosystem marker
- **US manufacturing access** via GlobalFoundries — relevant for defense/DoE
  programs post-CHIPS Act

### What Navitas doesn't have

- **Scale** — FY2025 $46M vs. WOLF ~$850M / ONMS power semi ~$1.5B / Infineon
  power ~€4B
- **Automotive qualifications at scale** — years behind WOLF, Infineon, STM
- **Pricing power** — SiC wafer prices falling, competitors have cost advantage
- **Exclusivity** — NVIDIA explicitly multi-sourcing

### Verdict: **Narrow moat, contested**

The GaN monolithic-integration story is real but commoditizing. The SiC
story is purely competitive. The NVIDIA relationship is validation but not a
recurring revenue moat.

---

## 6. Management & Leadership

- **CEO Gene Sheridan** — Co-founder, ex-International Rectifier, since inception.
  Technical founder; compensation heavy in equity (alignment mostly good but
  equity grants dilutive).
- **CFO Todd Glickman** — appointed 2023, ex-SiTime.

### Capital Allocation Track Record

- **5.3× share dilution** FY21→FY25 (39M → 206M shares)
- Cash raises timed opportunistically — $237M cash buildup in FY25 suggests a
  late-2025 equity raise into the NVIDIA-news rally (need 10-K for detail)
- GeneSiC acquisition (2022, ~$90M) — strategic but dilutive; integration
  acceptable, not great
- **Declining SBC** ($63M → $14.5M) — positive; discipline improving
- **Low-margin mobile exit** — painful but strategically correct

Verdict: **Technically credible, capital-discipline mediocre-to-improving**.
Execution on the pivot is the single largest risk — management has not yet
demonstrated ability to scale high-power sales to >$200M.

---

## 7. Strategic Growth Initiatives

### Near-term (2026)
1. **NVIDIA 800V HVDC**: Board-level co-development for "Kyber" rack systems
   powering Rubin Ultra GPUs. Revenue contribution: 2027+
2. **GlobalFoundries US GaN partnership**: Production start H2 2026,
   ramp 2027. Enables defense/hyperscale customers with US-sourcing needs
3. **Automotive OBC (On-Board Charger) design-wins** — disclosed but
   magnitude unclear

### Medium-term (2027–2028)
1. **Grid-scale SiC** (solid-state transformers) — multi-year design cycle
2. **Data center PSU share gains** — as hyperscalers adopt 54V→800V transition
3. **Industrial motor drives** — Infineon/ABB competition

### Long-term (2028+)
- **800V EV traction inverters** — if design-wins convert
- **Subsea / defense / aerospace** niche power — high-margin

---

## 8. Key Risks (Impact × Probability)

| Risk | Impact | Probability | Composite |
|------|:------:|:-----------:|:---------:|
| **Dilutive capital raise before FCF positive** | High | Medium (45%) | **High** |
| **NVIDIA design-win produces minimal revenue** | High | Medium (40%) | **High** |
| **SiC ASP decline faster than volume growth** | High | Medium (35%) | **High** |
| Larger competitors (WOLF, STM, Infineon) undercut pricing | Medium | High (55%) | High |
| Multiple compression as market reprices growth story | High | Medium (50%) | **High** |
| **CFO transition execution risk** *(NEW)* | Medium | Medium (35%) | **Medium-High** |
| US/China tariff or export control on GaN/SiC | Medium | Low (20%) | Medium |
| Technology substitution (next-gen silicon or GaN-on-Si breakthrough) | High | Low (15%) | Medium |

**Capital raise probability reduced (60% → 45%)**: Q1 cash $221M with ~$15.9M quarterly burn implies 3.5-year runway at current pace. Q1 beat and Q2 guide suggest ramp reducing burn — but high-power capacity investment may still require external funding in 2027.

**New risk — CFO transition**: Tonya Stevens replacing 10-year veteran Todd Glickman during a critical strategic pivot. Leadership change introduces near-term uncertainty on capital allocation priorities and investor communication continuity.

---

## 9. Industry-Specific Macro Analysis

### Wide-Bandgap Semiconductor Market

- Global WBG power semi market projected 17–34% CAGR through 2034 (industry
  reports)
- **GaN** — fastest-growing segment, but pricing pressure from Chinese entrants
- **SiC** — currently 10× GaN market size, slower growth but more automotive pull

### AI Datacenter Power Transition

- Current: 54V in-rack, 480V AC to facility
- Future (NVIDIA Kyber / Rubin Ultra era): 800V HVDC direct to rack
- Efficiency gain: ~5% end-to-end (significant at 100+ MW facility scale)
- Copper reduction: ~45% (BOM cost saving for hyperscalers)
- Adoption timeline: Design 2026, deployment 2027–2028, volume 2028–2030
- **Key point**: Even if NVIDIA wins, Navitas's revenue is 2+ years out

### Grid Modernization

- US IRA + EU grid package = $1T+ multi-decade tailwind
- SiC solid-state transformers relevant but 3–5 years from commercialization
- Navitas competes here, but not the leader

---

## 10. Valuation & Comparable Analysis

### Current Multiples (FY2025 basis)

| Metric | NVTS | Context |
|--------|-----:|---------|
| EV / Revenue (TTM) | **~88×** | vs. WOLF ~5×, ON ~3×, STM ~2× |
| P / E | N/A (loss) | — |
| P / S | **~93×** | Historic US semi average 4–6× |
| P / Tangible Book | ~15× | Most value in cash + IP |

### Comparable Small-Cap WBG / AI Power

| Ticker | Mkt Cap | Rev (TTM) | EV/Rev | Growth (TTM) |
|--------|--------:|----------:|-------:|-------------:|
| NVTS | $4.3B | $46M | 88× | –45% |
| WOLF (Wolfspeed) | ~$2B | ~$850M | ~5× | +20% |
| POWI (Power Integrations) | ~$4B | ~$420M | ~8× | +3% |
| ONMS (onsemi power) | ~$18B | ~$7B | ~2× | –10% |
| STMicro | ~$22B | ~$13B | ~1.7× | –15% |

**Observation**: NVTS trades at 17× WOLF's EV/Revenue multiple despite WOLF
being 18× larger in revenue, also AI-exposed, also with SiC, and actually
profitable at gross-margin line. The NVTS premium reflects 100% optionality,
not business fundamentals.

### Reverse-DCF / Growth Required To Justify $18.47

For current mcap ($4.26B) to be justified at a mature semiconductor multiple
(6× EV/Revenue, 20% operating margin, 15% WACC):
- Need ~$700M revenue (15× FY25) + sustained 20% operating margin
- At mgmt's current trajectory ($46M → maybe $80M 2026 → $150M 2027), this
  implies reaching $700M by 2029–2030
- **This is possible but requires NVIDIA-scale + grid + EV wins to all
  convert to revenue simultaneously**

**Honest assessment**: Current price requires bull-case assumptions to be
approximately correct. Any wobble in execution = severe multiple compression.

---

## 11. Position Building Strategy

### Current Stance (2026-07-10): No Position

Prior position entered 2026-05-07 (~$16 avg), peaked to $29.25 (May 22),
trailing stop $23.33 triggered. Position is **fully closed**.

Stock now at $13.47 — below the original entry zone ($14.50–$16.50) and in
Stage 3 correction. **Do not re-enter before Q2 earnings (Jul 27)**.

### Q2 Earnings Gate (Jul 27, 2026)

This is the next binary. Two paths:

| Outcome | Condition | Action |
|---------|-----------|--------|
| Q2 BEAT + strong Q3 guide | Revenue ≥$10.5M AND non-GAAP GM ≥ 39.5% AND Q3 guide ≥$11.5M | Run `/stock-entry NVTS` — evaluate Stage 2 re-entry if technical confirms |
| Q2 MISS | Revenue <$9.5M OR GM compression OR Q3 guide <$10M | Thesis-break triggered; avoid for 2+ quarters |
| Q2 IN-LINE, soft guide | Revenue $9.5–10.5M, Q3 guide $10–11M | Watch only; wait for Stage 2 re-establishment |

### If Re-entry Triggers Post-Q2

| Tranche | Trigger | Size | Form |
|---------|---------|-----:|------|
| 1 | Q2 beat + stock holds MA150 ($13.40 region) post-earnings | 0.5% | Stock |
| 2 | Breakout above MA50 (current $21; will be lower by Aug) on volume | 0.25% | Stock |
| 3 | First HVDC revenue quarter disclosed | 0.25% | Stock |

**Total cap**: 1% of portfolio. No position before Q2 earnings regardless of price.

### Options vs. stock

**Avoid calls pre-earnings** — IV will expand into Jul 27 earnings, risk of
IV crush on any result. If re-entering post-earnings, use stock only.

---

## 12. BAIT Framework (Mauboussin)

### B — Behavioral

**Sentiment diverging**. After the +81% run to $29.25 peak (May 22), retail
enthusiasm has cooled. X.com remains bullish (57% bull vs 15% bear) but
Reddit and news turn bearish (Reddit: 17% bull vs 22% bear; News: 27% bull
vs 64% bear). Short interest 16.1% of float — elevated, potential squeeze
fuel if Q2 beats. Today's −5% on 35.77× volume ratio suggests forced
selling / stop-outs, not fundamental revaluation.

Verdict: **Behavioral signal is mixed/slightly bearish. Elevated short interest is a contrarian positive if Q2 confirms thesis — short squeeze candidate**.

### A — Analytical

**Weak**. No reasonable DCF justifies $4.26B mcap on $46M revenue. Requires
bull-case execution to even match current price. Street estimates Q1 EPS
–$0.05 but no firm high-power revenue ramp modeled.

Verdict: **Analytical signal negative** — stock is priced for perfection.

### I — Informational

**Weak**. The NVIDIA partnership is extensively covered. The GlobalFoundries
partnership is press-released. Q4 earnings transcripts are public. No
meaningful informational asymmetry available to a retail / independent
analyst. This is not a "read the 10-K that nobody else read" situation.

Verdict: **Informational edge: minimal**.

### T — Technical

**Stage 3 correction. Not actionable.** Stock −54% from $29.25 peak.
Price $13.47 vs MA50 $21.00 (−35.9% below) — SEPA trend template fails
conditions 5 and 7. Critical support: MA150 $13.40 (price barely above) and
rising MA200 $12.51 (+7.7% above, +$1.32 in 1 month = strongly rising —
bullish longer-term signal). MA200 is the ultimate floor; if price breaks
below $12.51 on elevated volume, Stage 4 risk increases.

Pattern: None forming. In active distribution/correction.

Verdict: **SEPA Stage 3 — trend broken, no valid entry. Watch MA150/MA200 as floor; need new Stage 2 base post-Q2 earnings to re-enter**.

### BAIT Overall

**Weak overlap — I is now slightly positive (base case priced in), A is neutral, B is mixed, T is clearly negative (Stage 3)**. 

At $13.47, the analytical picture has shifted favorably vs. the original May 2026 analysis at $17.55: the stock now trades below PW EV ($16.30), meaning there is a modest margin of safety for the first time since initial coverage. However: T (Stage 3) is the hard SEPA block. The wiki's BAIT discipline requires T (Stage 2) before sizing in — even with favorable B/A/I, Stage 3 is a hard stop.

The prior +81% run validated the thesis framework. The current Stage 3 correction to original entry zone tests whether this is a "post-extension consolidation" (normal — rebase and re-enter in Stage 2) or "thesis break" (Q2 miss → exit).

---

## 13. Bull / Bear / Base Scenarios

### Bull Case (probability 20%) — Price target $30, +123% from $13.47

*(Reduced from 25% — Stage 3 breakdown shows market skepticism; re-entry timeline pushed out)*
- Q2 2026 beat ($10.5M+) triggers short squeeze + re-rating
- NVIDIA 800V HVDC ramps faster than expected; 2028 revenue contribution $100M+
- GlobalFoundries US GaN launches on schedule, unlocks defense / hyperscale
- 2027 revenue reaches $180–220M with >40% gross margins
- Market awards 15× EV/Revenue multiple on high-growth turnaround
- Implied $30 / share; ~$6.2B mcap

### Base Case (probability 55%) — Price target $16, +19% from $13.47

*(Probability raised from 50% — Q1 confirmed, Q2 guide $10M intact; sequential recovery remains on track)*
- Q2 revenue $9.8–$10.5M (meets guide); Q3 guide $11–12M confirms ramp
- Sequential ramp continues ($10M Q2 → $12–15M by Q4 2026)
- 2027 revenue $90–120M as HVDC begins contributing incrementally
- Still unprofitable; 2028 FCF near breakeven
- Multiple compresses to 25× EV/Revenue as growth story meets reality
- Implied $16 / share; ~$3.3B mcap

### Bear Case (probability 25%) — Price target $6, –55% from $13.47

*(Probability unchanged — Q2 miss risk real given Stage 3 breakdown + high vol today suggesting smart money concern)*
- Q2 2026 misses guide (<$9.5M) or Q3 guidance <$10M
- Mobile further decay; competitive displacement in SiC from Chinese vendors
- Dilutive capital raise at depressed price (2027)
- CFO transition disrupts investor relations or capital strategy
- Multiple compresses to 10× EV/Revenue at $80M run-rate
- Implied $6 / share; ~$1.3B mcap

### Probability-Weighted EV

**PW EV = (0.20 × $30) + (0.55 × $16) + (0.25 × $6) = $6.0 + $8.8 + $1.5 = ~$16.30**

*(Updated from $16.25 — minor probability shift, base case probability raised)*

**Current $13.47 vs. PW EV $16.30 → +21% implied upside — modest margin of safety for the first time since initial coverage.**

The stock now trades below PW EV for the first time since April initiation. However, Stage 3 technical breakdown overrides this modest fundamental discount — the SEPA framework prohibits entry until Stage 2 re-establishes. The margin of safety is fragile (Q2 miss collapses it immediately).

---

## 14. Bottom Line

### 1-year view (by 2027-07-10)
- **Base case**: $16 — Q2 meets guide, ramp confirms through 2026; stock recovers to PW EV
- **Trigger for upside**: Q2 ≥$10.5M + Q3 guide ≥$12M + HVDC pipeline milestone
- **Trigger for downside**: Q2 miss (<$9.5M) OR CFO stumble OR capital raise announcement

### 3-year view (by 2029-07-10)
- **Bull**: $40–50 if NVIDIA Kyber/Rubin era converts, Navitas captures 15%+ of NVIDIA power BOM
- **Base**: $15–20 if pivot executes but doesn't scale to compounder level
- **Bear**: $2–6 if capital raise + competitive displacement + HVDC delay

### Portfolio allocation recommendation
- **Current position**: **0%** — position was fully exited (trailing stop $23.33 triggered May–Jun 2026)
- **Re-entry gate**: Do NOT enter before Q2 earnings (Jul 27, 2026)
- **Post-Q2 re-entry target**: 0.5–1% if Q2 beat + Stage 2 re-establishes above MA150
- **Position form**: 100% stock (IV still elevated pre-earnings; avoid calls)
- **Next monitoring trigger**: Q2 2026 earnings — **July 27, 2026**

### Verdict
**Watch — No position. Q2 Jul 27 is the binary. First time stock trades below PW EV.**

The prior trade worked as designed: entered ~$16 (May 7), peak $29.25 (+81%), trailing stop $23.33 triggered. Stock has corrected to $13.47 — back below the original entry zone.

The fundamental thesis is STILL INTACT: Q1 beat ($8.6M), sequential ramp confirmed, Q2 guide $10M, cash runway 3.5+ years. The Stage 3 technical breakdown reflects multiple compression and profit-taking from the parabolic run, not thesis failure. Current price ($13.47) is actually below PW EV ($16.30) for the first time — modest margin of safety exists.

But Stage 3 is a hard stop per SEPA framework. The correct play: wait for Q2 earnings (Jul 27), verify thesis continuation, then evaluate fresh entry if stock re-establishes Stage 2 above MA150/MA200. Do not re-enter into a falling knife regardless of fundamental discount.

---

## 15. Monitoring Checklist

**Q1 2026 earnings — May 5, 2026** ✅ COMPLETE
- [x] Revenue ≥ $8.5M → **$8.6M** ✅
- [~] Gross margin ≥ 40% → **Non-GAAP 39.0%** (1ppt short; GAAP –9.3% due to intangibles)
- [x] Q2 guidance: $10M+ → **$10.0M ±0.5M** ✅
- [ ] FY2026 revenue guidance → **Not provided** (gap)
- [~] NVIDIA 800V HVDC timeline → GTC board demo; material revenue still 2027+
- [x] Capital raise language → **$221M cash, no raise signaled** ✅

**Trade cycle May–Jun 2026** ✅ COMPLETE
- [x] Entry $14.50–16.50 (May 7) → executed ~$16 avg
- [x] First trim 20% at $22.87 (May 11) → trailing stop raised to $18.00
- [x] Second trim 10% at $29.25 (May 22) → trailing stop raised to $23.33
- [x] Trailing stop $23.33 triggered → position fully closed (between May 22 – Jul 10)
- [x] Total return: +81% on the full run from the entry zone; realized portion locked by trailing stop

**⚡ Q2 2026 — July 27, 2026** ← NEXT CRITICAL BINARY (17 days)
- [ ] **Revenue ≥ $10.0M** (meet guide; below = thesis-break risk)
- [ ] **Revenue ≥ $10.5M** (beat; triggers potential short squeeze + re-entry eval)
- [ ] Non-GAAP GM ≥ 39.5% (continued expansion confirms pricing power)
- [ ] Q3 2026 guidance ≥ $11.5M (sequential acceleration confirmed)
- [ ] New CFO Tonya Stevens: any change in capital allocation language?
- [ ] HVDC pipeline update — first order pipeline disclosed?
- [ ] GlobalFoundries US GaN qualification progress update
- [ ] Short interest update (16.1% float → watch for squeeze setup)

**Mid-term triggers (Q3–Q4 2026)**
- [ ] Q3 2026 (~Nov): HVDC design-win pipeline → first datacenter revenue?
- [ ] Q4 2026 (~Feb 2027): $15M+ run-rate + 2027 guidance; GAAP GM turn positive?
- [ ] GlobalFoundries US GaN production launch (H2 2026)

**Re-entry conditions checklist (post-Q2 beat)**
- [ ] Q2 revenue ≥$10.5M AND non-GAAP GM ≥39.5% AND Q3 guide ≥$11.5M
- [ ] Price back above MA150 ($13.40 → will recalculate Aug)
- [ ] Stage 2 trend template re-establishes (≥6/8 conditions)
- [ ] SEPA valid base pattern forming (VCP or flat base ≥3 weeks)
- If all 4: run `/stock-entry NVTS` for fresh entry analysis

**Thesis-break triggers** (any ONE = reconsider entirely, no re-entry)
- Q2 2026 revenue miss (<$9.5M) — sequential recovery stalls
- Q3 guidance <$10M — H2 2026 ramp doesn't materialize
- Capital raise announcement at current or lower price
- NVIDIA shifts primary power supplier public
- Chinese GaN vendor (e.g., Innoscience) wins hyperscale contract
- Non-GAAP gross margin decline below 35% (pricing pressure materialized)

**Continuing thesis-strength triggers** (raise conviction if these occur)
- Q2 beat + Q3 guide ≥$12M → bull case probability raises to 30%
- First HVDC revenue disclosed, even small ($500K+)
- Short squeeze triggers (>20% intraday on volume + Q2 beat)
- GlobalFoundries US GaN receives defense/DoE qualification

---

## Sources

- Yahoo Finance: https://finance.yahoo.com/quote/NVTS — price, market cap, beta
- stockanalysis.com/stocks/nvts/ — FY2021–FY2025 income / cash flow / balance sheet
- Navitas IR: https://ir.navitassemi.com — NVIDIA 800V HVDC press release, Q4 2025 release
- stocktitan.net — Q4 2025 summary, NVIDIA partnership detail
- globenewswire (Navitas Feb 24, 2026) — FY2025 full-year results
- 24/7 Wall St / AAII — Q1 2026 consensus estimates
- `raw/analyses/chen.md` — Yun Chen 4/16 & 4/21 mentions

**Data gaps flagged for next session**:
- FY2025 10-K full geographic segment mix
- FY2025 revenue by end-market (precise percentages, not management commentary)
- Q1 2026 10-Q after May 5 report
- Detail on FY2025 equity raise (date, size, price)
