# DSEM — Domotics Structural Evaluation Model

**Open standard for assessing home automation proposals based on observable evidence, not marketing.**

![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)
![Version](https://img.shields.io/badge/Version-1.0.0-blue.svg)
![Status](https://img.shields.io/badge/Status-Stable-green.svg)
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
- [6. Validation Status](#6-validation-status)
- [7. How to Contribute](#7-how-to-contribute)
- [8. License](#8-license)
- [9. Acknowledgments](#9-acknowledgments)

---

## 1. WHY THIS EXISTS

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

---

## 2. THE 8 STRUCTURAL DIMENSIONS

Each dimension is scored **1 to 5** based on **observable evidence** (website, brochure, meeting answers, documentation).

---

### D1 — Infrastructure
*What are they actually building with?*

| Level | Evidence |
|-------|---------|
| 1 | Only WiFi / Bluetooth retail devices, no hub |
| 2 | Proprietary cloud ecosystem, mandatory app |
| 3 | Physical hub but no declared standard |
| 4 | Explicit open standards (Zigbee, KNX, Modbus, MQTT, DALI) |
| 5 | Wired bus / documented distributed architecture |

**Detector question:** *"What protocols do you use, and what other brands can I connect?"*

---

### D2 — Operational dependency
*What happens if the provider disappears?*

| Level | Evidence |
|-------|---------|
| 1 | System dies without their cloud |
| 2 | Works offline but cannot be reprogrammed |
| 3 | Only they can maintain it |
| 4 | Another integrator can take over |
| 5 | Client has full access + complete documentation |

**Detector question:** *"If you don't exist tomorrow, who fixes it?"*

---

### D3 — Functional depth
*What do they actually integrate?*

| Level | Evidence |
|-------|---------|
| 1 | Only lights and plugs |
| 2 | Lights + scenes |
| 3 | Lights + HVAC + security |
| 4 | Coordinated multi-system integration |
| 5 | Energy management + conditional logic + historical monitoring |

**Detector question:** *"Give me one example where two different systems talk to each other."*

---

### D4 — Value model
*What are they actually selling?*

| Level | Evidence |
|-------|---------|
| 1 | Device sales |
| 2 | Device + installation |
| 3 | Turnkey project |
| 4 | Custom engineering |
| 5 | Building infrastructure |

**Detector question:** *"How do you quote: per device, per hour, or per project?"*

---

### D5 — Structural complexity
*What does the installation require?*

| Level | Evidence |
|-------|---------|
| 1 | Plug & Play |
| 2 | Basic electrical installation |
| 3 | Dedicated electrical panel required |
| 4 | Requires technical project |
| 5 | Requires architectural planning |

**Detector question:** *"At what stage of construction do you get involved?"*

---

### D6 — Technological transparency
*Do they show or hide?*

| Level | Evidence |
|-------|---------|
| 1 | Only lifestyle marketing |
| 2 | Talks about "AI" with no architecture explanation |
| 3 | Describes general functionality |
| 4 | Publishes specific technologies and brands |
| 5 | Publishes schematics, protocols and architecture |

**Detector question:** *Look at their website for 30 seconds. Do you see technology or just pretty photos?*

---

### D7 — Ecosystem sustainability
*Does this exist in 10 years?*

| Level | Evidence |
|-------|---------|
| 1 | Models discontinued in <2 years |
| 2 | Single brand dependency |
| 3 | Open standard + captive hardware |
| 4 | Reprogrammable / replaceable hardware |
| 5 | Public documentation + community + multiple manufacturers |

**Detector question:** *"Where do I buy a spare part in 5 years?"*

---

### D8 — Privacy and data sovereignty
*Where is my data? Who can see it?*

| Level | Evidence |
|-------|---------|
| 1 | Mandatory cloud, foreign servers, hidden telemetry |
| 2 | Mandatory cloud with regional servers |
| 3 | Hybrid: local + optional cloud |
| 4 | Local by default, cloud optional and disableable |
| 5 | Local + open source / documented, zero telemetry |

**Detector question:** *"Does my data leave the country? Can you tell when I'm home?"*

---

## 3. CONTEXT WEIGHTING

DSEM allows weight adjustment based on region and client profile.

**Proposed weighting for Argentina / Latin America:**

| Dimension | Weight | Reason |
|----------|--------|--------|
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

## 4. STRUCTURAL PROFILES

| Profile | D1 | D2 | D7 | D8 | Typical Score | Description |
|---------|----|----|----|----|---------------|-------------|
| Red — Ultra light | 1-2 | 1-2 | 1-2 | 1 | 20-35 | Gadgets, mandatory cloud, disposable |
| Orange — Heavy closed | 4-5 | 2-3 | 2-3 | 2-3 | 45-65 | Professional but captive |
| Green — Open hybrid | 3-4 | 3-4 | 3-4 | 4 | 60-75 | Commodity hardware + custom firmware + local |
| Blue — Balanced architecture | 4 | 4-5 | 4-5 | 4-5 | 75-90 | Documented, maintainable, open standards |
| Black — Critical infrastructure | 5 | 5 | 5 | 5 | 90-100 | Industrial / hospital grade |

**DSEM does not say which profile is "better".**  
It says which profile each proposal fits.  
**The client decides what risk they are willing to take.**

---

## 5. COMPARISON MATRIX FOR TENDERS

| Criterion | Offer A | Offer B | Offer C | Offer D |
|-----------|---------|---------|---------|---------|
| Declared standard | Zigbee, MQTT, RF | Proprietary WiFi | KNX | Zigbee/MQTT/RF/LoRa |
| What devices can you connect? | Only their catalog | Only their brand | Any KNX | Any brand using the standard |
| Works without internet? | Yes | No | Yes | Yes |
| Spare parts in 5 years? | Only from them | No | Yes, imported | Yes, commodity |
| Do they hand over credentials? | No | No | Yes | Yes |
| Documentation | User manual | User manual | Drawings + specs | Drawings + topology + source code (if applicable) |
| DSEM Profile | Orange — Heavy closed | Red — Ultra light | Blue — Balanced | Green — Open hybrid |

---

## 6. VALIDATION STATUS

**Current version:** v1.0 — Foundational document.

**Next steps:**
- Evaluate 20 companies in local market.
- Publish anonymized case studies.
- Adjust criteria based on empirical evidence.
- Public launch with open license.

---

## 7. HOW TO CONTRIBUTE

This is an **open standard**. You can:

- Use it to evaluate proposals.
- Adapt it to your region (adjust weights).
- Translate it.
- Propose improvements via [GitHub Issues](https://github.com/cosolabs/dsem/issues).
- Share your evaluation cases (anonymized).

**We need:**
- Real world testing.
- Criticism.
- Edge cases that break the model.

---

## 8. LICENSE

**DSEM v1.0 — Domotics Structural Evaluation Model**  
© Matias Cacciagrano, 2025

**License:** [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)

- You may share and adapt.
- You must give credit.
- You must share improvements under the same license.
- Commercial use is allowed.

---

## 9. ACKNOWLEDGMENTS

This model was built from real world experience in the **Argentine market**, where import restrictions, currency volatility and lack of local technical support make vendor lock-in a critical risk.

It is inspired by:
- Open standards communities (Home Assistant, ESPHome, Tasmota).
- Architects and developers tired of proprietary "black boxes".
- Clients who just wanted their home to work, not to be a hostage.

---

**Version 1.0 — March 2025**  
[github.com/cosolabs/dsem](https://github.com/cosolabs/dsem)
