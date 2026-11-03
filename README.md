# 🌾 Fasal Flow

**Digitizing the Farm-to-Business Agricultural Supply Chain**

Fasal Flow is a B2B AgTech platform concept that connects farmers directly to wholesale buyers, food processors, retail chains and exporters. It replaces the opaque, multi-layer mandi system with AI-verified quality grading, escrow-backed contracts and instant farmgate payouts.

> Built by **Team Barbie** for a hackathon. This repository contains the interactive pitch website.

🔗 **Live site:** `https://YOUR-PROJECT.vercel.app` *(replace after deploying)*

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
| **AI + NIR quality grading** | Four-parameter Quality Index scored at the farmgate, bound to the purchase order |
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

## What is in the website

Interactive sections, all in one scrolling page:

- **Quality engine:** live QI calculator with gauge and automatic Grade A/B/C tiering
- **Mandi vs FasalFlow:** per-ton cost comparison with an adjustable crop value
- **Scale math:** adjustable FSP count and MT per FSP, shows GMV, revenue, contribution and run-rate
- **Business model:** nine blocks in order, each with expandable full detail
- **Go-to-market:** paid, organic, grassroots and technical-integration channels
- **vs e-NAM:** strengths, flaws, our answer and a head-to-head table
- **Technology, roadmap, team and contact**

## Project structure

```
fasalflow/
├── index.html            # Page markup
├── assets/
│   ├── css/style.css     # Theme, layout, responsive rules
│   └── js/main.js        # Calculators, tabs, nav, business-model blocks
├── docs/                 # Project documentation
│   ├── PROJECT_OVERVIEW.md
│   ├── BUSINESS_MODEL.md
│   ├── QUALITY_INDEX.md
│   ├── GO_TO_MARKET.md
│   └── ROADMAP.md
├── vercel.json           # Hosting config
├── LICENSE
└── README.md
```

## Run locally

No build step and no dependencies.

1. Download or clone the repo.
2. Double-click `index.html` to open it in a browser.

Or serve it locally:

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy for free on Vercel

1. Push this repo to GitHub.
2. On [vercel.com](https://vercel.com), sign in with GitHub and choose **Add New > Project**.
3. Import this repository and click **Deploy** (leave all settings at their defaults).

## Tech

Plain HTML, CSS and JavaScript. Fonts (Fraunces and Figtree) load from Google Fonts, with serif and sans-serif fallbacks if offline.

## Team

| Name | Role |
|---|---|
| **Hriman Das Gupta** | Lead Strategist and Operations |
| **Yuvraj Soni** | Lead Tech and Financial Architecture |

📧 fasalflowofficial@gmail.com

## Disclaimer

Figures such as take rate, unit economics and scale projections are illustrative targets from the hackathon pitch deck, not audited results.

## License

Released under the MIT License. See [LICENSE](LICENSE).
