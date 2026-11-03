# 🌾 Fasal Flow

**Digitizing the Farm-to-Business Agricultural Supply Chain**

Fasal Flow is a B2B AgTech platform concept that connects farmers directly to wholesale buyers, food processors, retail chains and exporters. It replaces the opaque, multi-layer mandi system with AI-verified quality grading, escrow-backed contracts and instant farmgate payouts.

🔗 **Live site: [fasal-flow.vercel.app](https://fasal-flow.vercel.app/)**

This repository contains the interactive pitch website, built for a hackathon.

---

## The problem

India's agricultural trade (USD 300B+) loses value at every step:

- **22%** post-harvest wastage
- **35%** cumulative middleman value leakage
- Produce passes through **5 to 7 intermediaries** before reaching a buyer
- Commission agents (Arhtiyas) charge **6% to 10%** interest-bound fees

## The solution

An asset-light, direct farmgate-to-buyer marketplace:

| Pillar | What it does |
|---|---|
| **AI + NIR quality grading** | Four-parameter Quality Index scored at the farmgate and bound to the purchase order |
| **Fasal Service Partners (FSPs)** | Village entrepreneurs act as micro-fulfilment managers for a fixed 1.5% to 2.0% fee |
| **Escrow + T+0 payouts** | Buyer funds locked before dispatch; farmer paid instantly at pickup |
| **Inclusive onboarding** | Voice IVR (Bhashini, 12+ dialects), WhatsApp audio, SMS and assisted village kiosks |
| **Smart logistics** | Full Truckload aggregation within a 15 km radius, route optimisation, e-way bills |

## Key numbers

| Metric | Value |
|---|---|
| Farmer share of trade value | **92%** (vs 79% in a traditional mandi) |
| Buyer cost reduction | **12 - 15%** |
| Farmer net realisation uplift | **24%** |
| Platform take rate | **6.0%** (3.0% transaction + 2.0% logistics + 1.0% instant settlement) |
| Revenue per metric ton | **₹1,200** (at ₹20,000/MT base value) |
| Extra income to farmer per MT | **₹2,600** (₹18,400 vs ₹15,800) |

## Quality Index (QI)

```
QI = (0.25 x Ac) + (0.35 x Mr) + (0.25 x Df) + (0.15 x Ht)
```

| Parameter | Meaning | Measured by |
|---|---|---|
| Ac | Appearance and size uniformity | Mobile camera computer-vision AI |
| Mr | Maturity and BRIX / moisture level | Handheld NIR spectrometer |
| Df | Defect and surface damage index | AI surface defect detection (inverted) |
| Ht | Harvesting delta timeliness | Days relative to optimal maturity window |

**Grades:** A (QI >= 85, premium export and retail), B (70 <= QI < 85, standard processing), C (QI < 70, local industrial processing).

## What is on the website

All sections are on one scrolling page, and four of them are interactive:

- **Quality engine:** live QI calculator with a gauge and automatic Grade A/B/C tiering
- **Mandi vs FasalFlow:** per-ton cost comparison with an adjustable crop value
- **Scale math:** adjustable FSP count and MT per FSP, showing GMV, revenue, contribution and run-rate
- **Business model:** nine blocks in order, each with expandable full detail
- **Also covered:** go-to-market channels, comparison with e-NAM, technology stack, roadmap, team and contact

## Run locally

No build step and no dependencies. Download or clone the repo and double-click `index.html` to open it in a browser.

Or serve it locally:

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Tech

Plain HTML, CSS and JavaScript in a single `index.html`. Fonts (Fraunces and Figtree) load from Google Fonts, with serif and sans-serif fallbacks if offline. Hosted on Vercel.

## Roadmap

| Phase | Timeline | Focus |
|---|---|---|
| 1 | Months 1 - 3 | Pilot in high-density agricultural belts, onboard 50 FSPs, stress-test the AI grading engine |
| 2 | Months 4 - 6 | Onboard 50+ corporate B2B buyers, integrate T+0 payout APIs, expand FPO collection hubs |
| 3 | Months 7 - 12 | Pan-India scaling, active arbitrage logistics routing, cross-border trade |

## Creators

| Name | Role |
|---|---|
| **Hriman Das Gupta** | Lead Strategist and Operations |
| **Yuvraj Soni** | Lead Tech and Financial Architecture |

📧 fasalflowofficial@gmail.com

## Disclaimer

Figures such as take rate, unit economics and scale projections are illustrative targets from the hackathon pitch deck, not audited results.
