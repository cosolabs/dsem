# DSEM — Domotics Structural Evaluation Model

## Towards a Standardized Framework for Architectural Assessment of Home Automation Systems

---

**Author:** Matias Cacciagrano  
**Year:** 2025  
**License:** CC BY-SA 4.0  
**Repository:** [github.com/cosolabs/dsem](https://github.com/cosolabs/dsem)  
**DOI:** 10.5281/zenodo.18613771  
**Status:** Version 1.1 — Conceptual Framework (Refined Version)

---

## Abstract

The home automation market has grown rapidly over the past decade, driven by the convergence of IoT, cloud computing, and mobile applications. However, the evaluation of domotics solutions is still primarily based on commercial or superficial functional criteria — brand recognition, price, user interface aesthetics — without systematically considering the underlying architecture, technological dependency, or structural sustainability of the ecosystem.

This paper introduces the **Domotics Structural Evaluation Model (DSEM)** , an open methodological framework designed to assess home automation solutions from an architectural and structural perspective. The model proposes **eight analytical dimensions**, each with observable and scoreable criteria on an ordinal scale (1-5), enabling objective comparisons between heterogeneous proposals. DSEM is neither software nor a commercial ranking: it is a **conceptual framework** aimed at professionalizing technical evaluation processes and reducing information asymmetry in the sector.

This document presents Version 1.1 of DSEM, a conceptual framework refined through empirical validation and peer feedback.

**Keywords:** Home Automation, Architectural Evaluation, Vendor Lock-in, Open Standards, Technological Sustainability, Data Sovereignty.

---

## 1. Introduction

Contemporary home automation is fragmented across multiple technological approaches that coexist — and compete — in the market: cloud-first solutions dependent on external servers, hybrid edge-cloud models, proprietary closed systems, open-standard implementations, and assistant-first integrations.

This fragmentation poses a structural problem for architects, developers, and end users: **there is no common language to compare technically heterogeneous proposals.** Decision-making is often based on easily available but poorly predictive variables: brand popularity, initial price, visual appeal, or non-verifiable functional promises.

These variables do not necessarily reflect operational resilience, dependency on the original provider, long-term spare parts availability, or effective user control over data. **DSEM emerges as a response to this methodological gap.**

---

## 2. State of the Art — Evaluation Models in Home Automation

### 2.1 Overview

The home automation sector has grown rapidly, driven by IoT, IP connectivity, and low-cost devices. However, technological development has focused on communication standards, automation platforms, and interoperability protocols — not on structural evaluation models.

### 2.2 Technical Standards and Protocols

Industrial standards such as Zigbee, Z-Wave, Thread, Matter, KNX, and BACnet define how devices communicate and ensure minimum interoperability levels.

**However, these standards do not evaluate the integrator's commercial model, measure operational dependency, or classify structural sustainability.** Their focus is technical, not strategic.

> **Micro-conclusion:** Technical standards regulate communication, but leave structural risk unaddressed.

### 2.3 Open Source Platforms

Platforms like Home Assistant, openHAB, and Domoticz have democratized home control, enabling expanded interoperability and reducing dependency on closed brands.

**However, they are technological infrastructures, not diagnostic models.** They facilitate integration but do not evaluate proposals.

> **Micro-conclusion:** Open source platforms empower users, but do not provide an evaluation framework.

### 2.4 Academic Evaluation Approaches

Academic literature includes research on IoT interoperability, energy performance, and multi-criteria decision methodologies (SAW, AHP). These are valuable for comparing specific technologies.

**However, they are not oriented toward the real market of integrators, do not analyze commercial obsolescence risk, and do not consider regional dependency.**

> **Micro-conclusion:** Academic approaches study components, not complete commercial proposals.

### 2.5 Identified Gap

The analysis reveals a clear gap: extensive development exists in protocols, technical architectures, and platforms — but no structural model exists that evaluates complete domotics proposals, classifies commercial architectural profiles, measures provider dependency, or enables objective comparison based on observable evidence.

### 2.6 DSEM Positioning

DSEM positions itself as a typological and diagnostic framework oriented toward the structural evaluation of domotics proposals, independent of brand, technology, or scale. Its differential contribution lies in multidimensional evaluation, non-hierarchical classification, real commercial applicability, and consideration of regional context.

### 2.7 State of the Art Conclusion

Existing standards regulate communication, platforms facilitate integration, and academic literature studies performance — but there is no public, open, market-applicable structural model that classifies complete proposals according to risk, dependency, and sustainability. **DSEM is proposed to fill this gap.**

---

## 3. Research Problem

The absence of structured evaluation frameworks leads to:

- Decisions based on marketing rather than architecture
- Impossibility of objective tendering between heterogeneous solutions
- Orphaned systems and hidden costs due to unidentified structural risks
- Chronic information asymmetry between providers and buyers

Product certifications and electrical regulations exist, but none address the problem from the evaluator's perspective.

---

## 4. Model Objectives

| Objective | Description |
|----------|-------------|
| **O1** | Provide a structural evaluation framework based on observable evidence |
| **O2** | Standardize comparative criteria between heterogeneous solutions |
| **O3** | Introduce ordinal metrics (1-5) per dimension, replicable and auditable |
| **O4** | Facilitate RFP and technical analysis processes |
| **O5** | Promote architectural transparency as a differentiating value |

The model does not establish a universal hierarchy, but rather typifies structural profiles so decision makers can consciously choose their risk level.

---

## 5. Methodology

DSEM defines **eight structural dimensions of analysis**. Each dimension is evaluated on an **ordinal scale from 1 to 5**, based exclusively on **observable evidence**.

### 5.1 Methodological Principles

1. **Observability:** Only facts verifiable at the time of assessment
2. **Ordinality:** The 1-5 scale reflects increasing degrees of structural maturity
3. **Modularity:** Dimensions are independent and can be weighted by context
4. **Openness:** Public, modifiable, and evolutionary under CC BY-SA 4.0

### 5.2 Model Dimensions

The eight dimensions emerged from a multi-source construction process:

- **Literature review** of academic and technical evaluation frameworks (see Section 2)
- **Market analysis** of 30+ commercial proposals from the Argentine home automation sector
- **Semi-structured interviews** with 5 architects and 8 homeowners about post-installation problems
- **Mapping** against existing standards: ISO 27001 (privacy), KNX and open protocols (infrastructure)

This process ensures the dimensions are empirically grounded, not theoretically imposed.

#### D1 — Technological Infrastructure
*Type of architecture, use of open standards, declared interoperability.*

| Level | Observable Evidence |
|-------|---------------------|
| 1 | Only WiFi/Bluetooth retail devices, no central hub |
| 2 | Proprietary ecosystem with mandatory cloud |
| 3 | Physical hub but no declared standard |
| 4 | Explicit open standards (Zigbee, KNX, Modbus, MQTT, DALI) |
| 5 | Wired bus / documented distributed architecture |

**Detector question:** *"What protocols do you use, and what other brands can I connect?"*

---

#### D2 — Operational Dependency
*Level of functionality without external servers or original provider.*

| Level | Observable Evidence |
|-------|---------------------|
| 1 | System dies without the provider's cloud |
| 2 | Works offline but cannot be reprogrammed |
| 3 | Only the original provider can maintain it |
| 4 | Another integrator can take over the project |
| 5 | Client has full access + transferable documentation |

**Detector question:** *"If you don't exist tomorrow, who fixes it?"*

---

#### D3 — Functional Depth
*Real automation capability beyond simple actions.*

| Level | Observable Evidence |
|-------|---------------------|
| 1 | Only lighting and plug control |
| 2 | Lighting + predefined scenes |
| 3 | Lighting + HVAC + security |
| 4 | Coordinated multi-system integration |
| 5 | Energy management + conditional logic + historical monitoring |

**Detector question:** *"Give an example where two different systems talk to each other."*

---

#### D4 — Value Model
*Nature of the value offered.*

| Level | Observable Evidence |
|-------|---------------------|
| 1 | Device sales (commodity) |
| 2 | Device sales + installation |
| 3 | Turnkey project |
| 4 | Custom engineering |
| 5 | Building infrastructure |

**Detector question:** *"How do you quote: per device, per hour, or per project?"*

---

#### D5 — Structural Complexity
*Technical level required for implementation.*

| Level | Observable Evidence |
|-------|---------------------|
| 1 | Plug & Play |
| 2 | Basic electrical installation |
| 3 | Dedicated electrical panel required |
| 4 | Requires prior technical project |
| 5 | Requires architectural planning |

**Detector question:** *"At what stage of construction do you get involved?"*

---

#### D6 — Technological Transparency
*Public documentation, APIs, accessible specifications.*

| Level | Observable Evidence |
|-------|---------------------|
| 1 | Only lifestyle marketing |
| 2 | Talks about "AI" with no architecture explanation |
| 3 | Describes general functionality |
| 4 | Publishes specific technologies and brands |
| 5 | Publishes schematics, protocols and architecture |

**Detector question:** *Look at their website for 30 seconds. Do you see technology or just photos?*

---

#### D7 — Ecosystem Sustainability
*Community, support, product lifecycle, spare parts.*

| Level | Observable Evidence |
|-------|---------------------|
| 1 | Models discontinued in <2 years |
| 2 | Single brand dependency |
| 3 | Open standard + captive hardware |
| 4 | Reprogrammable / user-replaceable hardware |
| 5 | Public documentation + active community + multiple manufacturers |

**Detector question:** *"Where do I buy a spare part in 5 years?"*

---

#### D8 — Privacy and Data Sovereignty
*User control over data, server location, telemetry.*

| Level | Observable Evidence |
|-------|---------------------|
| 1 | Mandatory cloud, foreign servers, hidden telemetry |
| 2 | Mandatory cloud with regional servers |
| 3 | Hybrid: local + optional cloud |
| 4 | Local by default, cloud disableable |
| 5 | Local + open source / documented, zero telemetry |

**Detector question:** *"Does my data leave the country? Can you tell when I'm home?"*

### 5.3 Scoring Protocol

To ensure consistent application across different evaluators:

| Question | Answer |
|----------|--------|
| **Can there be ties?** | Yes. Two proposals can obtain the same score. In case of a tie, the evaluator must briefly document why both are considered at the same level. |
| **Are intermediate scores allowed?** | No. The scale is strictly ordinal with integer values from 1 to 5. Half points are not permitted. Observable evidence rarely admits fine nuances. |
| **What if there is no information?** | Default score = 1. Absence of evidence is evidence of opacity. If information is deliberately hidden, the lowest level is assumed. |
| **Simple or weighted average?** | Both. Simple average per dimension for internal consistency, then weighted average according to regional context (see Section 3). |
| **Cross-validation?** | Recommended for high-value tenders (> USD 10,000). Two independent evaluators should score separately and average results. Discrepancies >1 point require calibration. |

---

## 6. Operational Structure

| Tool | Function | Audience |
|------|---------|----------|
| **Architect's Checklist** | Ready-to-copy text for tender specifications | Prescribers |
| **Comparison Matrix** | Evaluation matrix with adjustable weighting | Technical evaluators |
| **Supplier Self-Assessment Form** | Sworn declaration for providers | Buyers |
| **Developer's Guide** | Translation of technical risk into resale value | Real estate developers |

All tools are publicly accessible under CC BY-SA 4.0.

---

## 7. Discussion

### 7.1 Conceptual Contribution

| Traditional Evaluation | DSEM Evaluation |
|-----------------------|-----------------|
| Brand-based | Architecture-based |
| Initial price-based | Structural risk-based |
| Functional promises-based | Observable evidence-based |
| Impossible comparison | Standardized typological comparison |

### 7.2 Limitations

| Limitation | Implication |
|-----------|-------------|
| Dependence on accessible information | Cannot evaluate what is deliberately hidden |
| Residual subjectivity | Requires minimum evaluator training |
| Cybersecurity excluded | Requires specific framework |
| LATAM-focused weighting | Requires regional adaptation |

---

## 8. Empirical Validation

### 8.1 Context

**Public building, 6000 m², 2021-2024.** Maintenance budget: 0.

Faced with zero budget for infrastructure maintenance, the in-house R&D department had to build, from scratch, a monitoring and control system for critical infrastructure using only:
- Discontinued components from old programs
- Recycled hardware
- Open source software
- In-house developed logic

**This project served as the first real-world test of the DSEM framework**, allowing retrospective evaluation of 12 subsystems and prospective validation of the model's predictive capacity.

### 8.2 The six layers (chronological order)

| Layer | Problem | Solution | Key dimensions |
|-------|---------|----------|----------------|
| 1 | Data center national signals without monitoring | OpenHAB + ESP32 | D1, D2, D7, D8 |
| 2 | OpenHAB doesn't scale | Custom stack: MQTT + Node-RED + Influx + Grafana | D1, D5, D7 |
| 3 | Water tanks (6000L each) without control | Sensors + night pattern logic | D3, D5 |
| 4 | Sewage pumps (sanitary risk) | Time-based protection in Node-RED | D2, D3, D7 |
| 5 | Rooftop HVAC (common areas) | 10 custom thermostats with ESP32 | D1, D3, D5 |
| 6 | Emergency doors misused as shortcuts | Magnetic sensors + alerts | D1, D3, D6 |

### 8.3 What we learned (dimension by dimension)

#### D1 — Infrastructure
**What happened:** Started with OpenHAB, migrated to ESP32 + MQTT, added Node-RED, InfluxDB, Grafana, built 10 thermostats, added magnetic sensors.
**What we learned:** When everything is open, nothing ties you down. You can change platforms, recycle hardware, modify logic.

#### D2 — Operational dependency
**What happened:** No provider. We were the provider. When OpenHAB didn't scale, we changed it. External biometric system kept existing alongside.
**What we learned:** Zero dependency is the only way to survive when the context is uncertain.

#### D3 — Functional depth
**What happened:** Data center + water tanks + sewage pumps + rooftop HVAC + emergency doors.
**What we learned:** Depth is how many different systems you can make talk to each other.

#### D4 — Value model
**What happened:** Sold nothing, bought nothing new. Value was in the logic we programmed.
**What we learned:** When budget is zero, hardware stops mattering. The only thing that counts is what you can do with what you have.

#### D5 — Structural complexity
**What happened:** Thermostats without modifying wiring, pump protection without touching panels, doors with magnetic sensors, custom stack requiring understanding of databases and MQTT.
**What we learned:** Complexity is understanding how each system works to add intelligence without breaking it.

#### D6 — Technological transparency
**What happened:** Grafana dashboards visible to all, own code, internal documentation. Security staff knew doors were monitored and stopped misusing them.
**What we learned:** Transparency changes behavior.

#### D7 — Sustainability over time
**What happened:** Recycled components, ESP32s still working, MQTT/Node-RED/Influx/Grafana with active communities.
**What we learned:** Sustainability is choosing technologies with community, standards, and alternatives.

#### D8 — Privacy and data sovereignty
**What happened:** Everything local, zero cloud, zero telemetry. Data never left the building. No subscriptions, no external servers.
**What we learned:** When your data is yours, no one can take it, charge you to see it, or know what happens in your building.

### 8.4 Validation conclusion

DSEM does not describe a theoretical ideal. It describes what actually worked for three years (2021-2024) in a 6000 m² public building with zero budget, facing critical infrastructure failures, sanitary risks, energy waste, and staff behavior problems.

**Every DSEM dimension was validated by facts, not assumptions.**

> If this worked in an Argentine public building between 2021 and 2024, with everything against it, it can work anywhere.

---

## 9. Implications for the Sector

1. **Raising the technical standard** in evaluation processes
2. **Professionalization of decision-making** for architects and developers
3. **Reduction of information asymmetries** for end clients
4. **Foundation for structural certifications** (non-commercial technical seal)

---

## 10. Future Work

| Line | Description | Status |
|------|-------------|--------|
| **Empirical validation** | Evaluation of 20 companies in local market | Pending |
| **Mathematical formalization** | Weighting system with parametric sensitivity | Pending |
| **Digital tool** | Interactive comparison matrix (Web/Sheets) | In development |
| **Regional adaptation** | Differentiated weightings for other markets | Pending |
| **Integration with existing frameworks** | Cross-mapping with KNX, Zigbee, Matter | Pending |

The model is published in version 1.1 as a conceptual framework with preliminary empirical validation.

---

## 11. Conclusion

DSEM constitutes a conceptual framework for evaluating home automation solutions from a structural and architectural perspective, shifting the focus from marketing toward sustainability, user sovereignty, and technical maturity.

In doing so, it contributes to professionalizing the relationship between providers and prescribers, equipping clients with tools to make informed decisions, and establishing a common language where fragmentation currently reigns.

Its open, collaborative nature allows any sector actor to use, critique, and improve it. The model is offered as a foundational structure, open to empirical testing and collaborative improvement by the academic and professional community.

---

## Acknowledgments

This model was built from direct experience in the Argentine market, where import restrictions, currency volatility, and scarcity of local technical support turn vendor lock-in into a structural risk.

Inspired by open standards communities (Home Assistant, ESPHome, Tasmota, OpenHAB), architects tired of proprietary black boxes, and clients who wanted their home to work.

Special thanks to the in-house R&D team that, between 2021 and 2024, proved that with open tools and engineering criteria, critical infrastructure can be maintained even with zero budget.

---

## References

[1] KNX Association. *KNX Specifications – System Specifications*, 2024.

[2] Connectivity Standards Alliance. *Matter Specification Version 1.3*, 2024.

[3] Zigbee Alliance. *Zigbee PRO Specification*, 2023.

[4] Home Assistant. *Open Source Home Automation Platform*, 2025.

[5] ESPHome. *ESPHome — Device Configuration for Home Automation*, 2025.

[6] Tasmota. *Tasmota — Open Source Firmware for ESP Devices*, 2025.

[7] Saaty, T. L. *The Analytic Hierarchy Process*. McGraw-Hill, 1980.

[8] Hwang, C. L. & Yoon, K. *Multiple Attribute Decision Making*. Springer, 1981.

[9] Zanella, A. et al. *"Internet of Things for Smart Cities"*. IEEE IoT Journal, 2014.

[10] Al-Fuqaha, A. et al. *"IoT: A Survey on Enabling Technologies"*. IEEE Com. Surveys, 2015.

[11] Guinard, D. & Trifa, V. *Building the Web of Things*. Manning, 2016.

[12] IRAM. *IRAM AEA 90364 – Instalaciones eléctricas*, 2021.

[13] IEC. *IEC 60364 – Low-voltage electrical installations*, 2020.

[14] Creative Commons. *CC BY-SA 4.0 License*, 2025.

[15] OpenHAB Foundation. *openHAB – Empowering the Smart Home*, 2025.

[16] Domoticz. *Domoticz – Open Source Home Automation*, 2025.

[17] CENELEC. *EN 50090 – Home and Building Electronic Systems*, 2022.

[18] ISO/IEC. *ISO/IEC 14543-3 – HES architecture*, 2020.

[19] BSI. *BSI PAS 212 – IoT device commissioning*, 2021.

[20] Mattern, F. & Floerkemeier, C. *"From the Internet of Computers to the Internet of Things"*. Informatik-Spektrum, 2010.

---

**Version 1.1 — March 2025**  
[github.com/cosolabs/dsem](https://github.com/cosolabs/dsem)  
**DOI:** 10.5281/zenodo.18613771

---

**License: CC BY-SA 4.0**  
Free use with attribution. Share improvements under same license. Commercial use allowed.
