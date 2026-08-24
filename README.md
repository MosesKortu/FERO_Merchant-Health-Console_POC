<div align="center">

# FERO · Merchant Health Console

**An interactive prototype for a Technical Product Owner case study.**

One console. Three merchant problems. The same way of working across all of them —
from reacting to fires to building a product that quietly protects itself.

<br>

![HTML5](https://img.shields.io/badge/HTML-5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS-3-1572B6?style=flat&logo=css3&logoColor=white)
![Chart.js](https://img.shields.io/badge/Chart.js-v4.0-FF6384?style=flat&logo=chartdotjs&logoColor=white)
![Zero Dependencies](https://img.shields.io/badge/dependencies-0-success?style=flat)
![Runs Offline](https://img.shields.io/badge/mode-offline-blue?style=flat)

<br>

> [!IMPORTANT]
> **This is a demonstration mockup, not a real product.**
> It is **not** connected to FERO, to any live system, API, database, or payment gateway.
> Every number, chart, file name, and merchant shown here is **illustrative sample data**,
> hand-authored to show *how* a monitoring console could work — not real FERO data.

</div>

<br>

---

## What this is

This repository holds a single, self-contained web page built as part of a **Technical Product Owner
case study for FERO**. It turns a written strategy memo into something you can actually click through.

The console walks through three merchant problems posed in the case brief, and shows how each one
would be diagnosed and prevented:

| Tab | Problem | What the console shows |
|-----|---------|------------------------|
| **Q1** | Merchants leaving over reconciliation numbers that don't match their books | A first-week diagnosis, a cause breakdown, and the safe-release checks for every future fee change |
| **Q2** | A Magento plugin that keeps breaking during onboarding | Where merchants get stuck, and a data-ranked list of the riskiest files to fix first |
| **Q3** | Urgent requests that break the sprint mid-flight | A 15-minute triage flow and a set of clear lanes so response depends on the issue, not the loudest voice |

<br>

## What this is **not**

To be completely clear, since it's designed to *look* like a real operational tool:

- ❌ It is **not** affiliated with, endorsed by, or connected to FERO or any of its systems.
- ❌ It does **not** read, write, or connect to any API, database, gateway, or backend of any kind.
- ❌ The metrics (`$142.6k`, `14.2%`, `18 hrs`, file names like `CheckoutObserver.php`, etc.) are **invented sample data** for illustration.
- ❌ Nothing here processes real payments, real merchants, or real money.

It is a **front-end mockup** — a picture of a product that runs entirely in your browser.

<br>

## Running it

There is nothing to install and nothing to build.

```bash
# Option 1 — just open the file
open FERO_Command_Center.html        # macOS
start FERO_Command_Center.html       # Windows
xdg-open FERO_Command_Center.html    # Linux
```

Or double-click `FERO_Command_Center.html` in any file browser. It opens in any modern browser,
**online or offline** — the charting library is bundled directly into the file, so it needs no internet
connection once downloaded.

<br>

## What you can click

- **Three tabs** — one per merchant problem (Q1 / Q2 / Q3).
- **Platform filter** (Q1) — switch between *All · Magento · Shopify · Custom API* and watch the
  discrepancy figure, the ledger chart, and the cause breakdown recalculate live.
- **Live charts** — built with Chart.js, styled to match FERO's look.
- **Status checks and risk rankings** — the pass/fail quality gates and the file-by-file risk scores.

All interactivity is client-side. Refreshing the page resets everything to its starting state.

<br>

## How it's built

```
FERO_Command_Center.html     ← the entire prototype, one file
│
├── HTML structure           three tab views, cards, tables
├── inline CSS               FERO palette · Inter + JetBrains Mono · responsive grid
├── inline Chart.js          bundled so it works with no internet
└── inline JavaScript        tab switching · platform filter · sample data
```

**Design system**

| Token | Value |
|-------|-------|
| Primary | Indigo `#4F46E5` |
| Base | White `#FFFFFF` / Ink `#0A0A0A` |
| Signals | Success `#059669` · Warning `#D97706` · Danger `#DC2626` |
| Type | Inter (text) · JetBrains Mono (figures) |
| Radius | 12px cards · 8px controls |

Everything lives in one file on purpose: it's meant to be handed over, opened, and clicked with zero setup.

<br>

## The wider case study

This console is the interactive piece of a three-part deliverable:

- 📄 **Strategy memo** — the full written plan for the three problems (Word document)
- 📊 **Slide deck** — a six-slide walk-through of the approach (PowerPoint)
- 🖥️ **This console** — the same plan, made clickable

<br>

## Credits

Designed and built by **Moses Bargue Kortu Jr.**
MSc, Business Analytics & Big Data · IE University

<br>

---

<div align="center">
<sub>

**Disclaimer** · This is an independent case-study prototype created for interview purposes.
"FERO" is referenced only as the subject of the case study. This project is a mockup with
sample data and is not connected to any real system, product, or company.

</sub>
</div>
