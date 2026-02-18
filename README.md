# DSEM — Domotics Structural Evaluation Model

**Open standard for assessing home automation proposals based on observable evidence, not marketing.**

![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)
![Version](https://img.shields.io/badge/Version-1.1.0-blue.svg)
![Status](https://img.shields.io/badge/Status-Refined%20Version-green.svg)
[![GitHub issues](https://img.shields.io/github/issues/cosolabs/dsem)](https://github.com/cosolabs/dsem/issues)
[![GitHub stars](https://img.shields.io/github/stars/cosolabs/dsem)](https://github.com/cosolabs/dsem/stargazers)

**Author:** Matias Cacciagrano — 2025  
**License:** [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)  
**Repository:** [github.com/cosolabs/dsem](https://github.com/cosolabs/dsem)  

---

## Table of Contents

- [1. Why This Exists](#1-why-this-exists)
- [2. The 8 Structural Dimensions](#2-the-8-structural-dimensions)
- [3. Context Weighting](#3-context-weighting)
- [4. Structural Profiles](#4-structural-profiles)
- [5. Comparison Matrix for Tenders](#5-comparison-matrix-for-tenders)
- [6. Real-world Validation](#6-real-world-validation)
- [7. Tools](#7-tools)
- [8. How to Contribute](#8-how-to-contribute)
- [9. License](#9-license)
- [10. Acknowledgments](#10-acknowledgments)

---

## 1. Why This Exists

The home automation market is broken.

Clients compare prices but **cannot compare risk**.  
Integrators compete against gadget sellers who look *"the same, but cheaper"*.  
Marketing departments sell "AI", "smart", "ecosystem" — but nobody explains **what happens when the internet goes down, when the company disappears, or when a device breaks 5 years later.**

**DSEM is not a ranking of "best domotics".**  
It is a **diagnostic tool to reveal structural risk.**

It measures:

- **Infrastructure** — What are you actually installing?
- **Operational dependency** — Who owns this system after installation?
- **Sustainability** — Can you buy spare parts in 5 years?
- **Privacy** — Where does your data go?
- **Transparency** — Do they show schematics or just lifestyle photos?

👉 [Read the full whitepaper →](whitepaper.md)

---

## 2. The 8 Structural Dimensions

| Dimension | What it measures |
|-----------|------------------|
| **D1 — Infrastructure** | Open standards vs black boxes |
| **D2 — Operational dependency** | What happens if the provider ceases to exist? |
| **D3 — Functional depth** | Real integration beyond lights and plugs |
| **D4 — Value model** | Do they sell devices or solutions? |
| **D5 — Structural complexity** | Plug & play or architectural planning? |
| **D6 — Technological transparency** | Do they show technology or hide behind marketing? |
| **D7 — Ecosystem sustainability** | Does this exist in 10 years? |
| **D8 — Privacy and data sovereignty** | Where does your data go? |

Each dimension is scored **1 to 5** based on **observable evidence** (website, brochure, meeting answers, documentation).

👉 [See detailed scoring criteria →](whitepaper.md#5-methodology)

---

## 3. Context Weighting (example: Argentina / Latin America)

| Dimension | Weight | Reason |
|-----------|--------|--------|
| D2 (Dependency) | 25% | Country risk = technical risk |
| D8 (Privacy) | 20% | Data sovereignty is critical |
| D1 (Infrastructure) | 15% | Technical foundation |
| D7 (Sustainability) | 15% | Spare parts + community |
| D3 (Functionality) | 10% | What the client thinks matters |
| D6 (Transparency) | 8% | Symptom, not cause |
| D5 (Complexity) | 5% | Correlated with D1 |
| D4 (Value model) | 2% | Describes business, not risk |

**Maximum weighted score: 100 points.**

---

## 4. Structural Profiles

| Profile | D1 | D2 | D7 | D8 | Typical Score | Description |
|---------|----|----|----|----|---------------|-------------|
| **Red — Ultra light** | 1-2 | 1-2 | 1-2 | 1 | 20-35 | Gadgets, mandatory cloud, disposable |
| **Orange — Heavy closed** | 4-5 | 2-3 | 2-3 | 2-3 | 45-65 | Professional but captive |
| **Green — Open hybrid** | 3-4 | 3-4 | 3-4 | 4 | 60-75 | Commodity hardware + custom firmware + local |
| **Blue — Balanced architecture** | 4 | 4-5 | 4-5 | 4-5 | 75-90 | Documented, maintainable, open standards |
| **Black — Critical infrastructure** | 5 | 5 | 5 | 5 | 90-100 | Industrial / hospital grade |

DSEM does not say which profile is "better".  
**The client decides what risk they are willing to take.**

---

## 5. Comparison Matrix for Tenders

| Criterion | Offer A | Offer B | Offer C | Offer D |
|-----------|---------|---------|---------|---------|
| Declared standard | Zigbee, MQTT | Proprietary WiFi | KNX | Zigbee/MQTT |
| Works without internet? | Yes | No | Yes | Yes |
| Spare parts in 5 years? | Only from them | No | Yes, imported | Yes, commodity |
| Documentation | User manual | User manual | Drawings + specs | Drawings + source |
| DSEM Profile | Orange | Red | Blue | Green |

👉 [Download comparison template →](comparativa-ofertas.md)

---

## 6. Real-world Validation

DSEM is not theory. Between 2021 and 2024, it was applied in a **6000 m² public building with zero budget** to:

- **Monitor** a data center hosting national public signals
- **Protect** sewage pumps from burnout (sanitary risk)
- **Control** HVAC with 10 custom-built thermostats
- **Detect** water leaks by analyzing night patterns
- **Prevent** emergency doors from being misused as shortcuts

👉 [Read the full case study →](case-studies/public-building-2021-2024.md)

---

## 7. Tools

| Tool | Function | Audience |
|------|----------|----------|
| **Architect's Checklist** | Ready-to-copy text for tender specifications | Prescribers |
| **Comparison Matrix** | Evaluation matrix with adjustable weighting | Technical evaluators |
| **Supplier Self-Assessment Form** | Sworn declaration for providers | Buyers |
| **Developer's Guide** | Translation of technical risk into resale value | Real estate developers |

All tools are **publicly accessible, modifiable, and evolutionary**, under CC BY-SA 4.0.

---

## 8. How to Contribute

This is an **open standard**. You can:

- Use it to evaluate proposals
- Adapt it to your region (adjust weights)
- Translate it
- Propose improvements via GitHub Issues
- Share your evaluation cases (anonymized)

**We need:**
- Real world testing
- Criticism
- Edge cases that break the model

---

## 9. License

**DSEM v1.1 — Domotics Structural Evaluation Model**  
© Matias Cacciagrano, 2025

**License:** [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)  
Free use with attribution. Share improvements under same license. Commercial use allowed.

---

## 10. Acknowledgments

This model was built from direct experience in the **Argentine market**, where import restrictions, currency volatility, and scarcity of local technical support turn vendor lock-in into a structural risk.

Inspired by:

- Open standards communities (Home Assistant, ESPHome, Tasmota, OpenHAB)
- Architects and developers tired of proprietary "black boxes"
- Clients who just wanted their home to work

Special thanks to the **in-house R&D team** that, between 2021 and 2024, proved that with open tools and engineering criteria, critical infrastructure can be maintained even with zero budget.

---

**Version 1.1 — March 2025**  
[github.com/cosolabs/dsem](https://github.com/cosolabs/dsem)
