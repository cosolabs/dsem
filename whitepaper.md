# DSEM — Domotics Structural Evaluation Model

## Towards a Standardized Framework for Architectural Assessment of Home Automation Systems

---

**Author:** Matias Cacciagrano  
**Year:** 2025  
**License:** CC BY-SA 4.0  
**Repository:** [github.com/cosolabs/dsem](https://github.com/cosolabs/dsem)  
**DOI:** Pending  
**Status:** Version 1.0 — Foundational Document

---

## Abstract

The home automation market has grown rapidly over the past decade, driven by the convergence of IoT, cloud computing, and mobile applications. However, the evaluation of domotics solutions is still primarily based on commercial or superficial functional criteria — brand recognition, price, user interface aesthetics — without systematically considering the underlying architecture, technological dependency, or structural sustainability of the ecosystem.

This paper introduces the **Domotics Structural Evaluation Model (DSEM)** , an open methodological framework designed to assess home automation solutions from an architectural and structural perspective. The model proposes **eight analytical dimensions**, each with observable and scoreable criteria on an ordinal scale (1-5), enabling objective comparisons between heterogeneous proposals. DSEM is neither software nor a commercial ranking: it is a **conceptual framework** aimed at professionalizing technical evaluation processes and reducing information asymmetry in the sector.

**Keywords:** Home Automation, Architectural Evaluation, Vendor Lock-in, Open Standards, Technological Sustainability, Data Sovereignty.

---

## 1. Introduction

Contemporary home automation is fragmented across multiple technological approaches that coexist — and compete — in the market: cloud-first solutions dependent on external servers, hybrid edge-cloud models, proprietary closed systems, open-standard implementations, and assistant-first integrations (Alexa, Google Home), among others.

This fragmentation poses a **structural problem** for architects, real estate developers, facility managers, and end users: **there is no common language to compare technically heterogeneous proposals.**

In practice, decision-making is often based on easily available but poorly predictive variables of architectural quality:

- Brand popularity.
- Initial purchase price.
- Visual appeal of the user interface.
- Non-verifiable functional promises ("artificial intelligence", "ecosystem", "future-proof").

These variables, however, **do not necessarily reflect** operational resilience, dependency on the original provider, long-term spare parts availability, effective user control over their own data, or the ability to be maintained by third parties.

**DSEM emerges as a response to this methodological gap.**

---

## 2. State of the Art — Evaluation Models in Home Automation and Smart Homes

### 2.1 Overview

The home automation and smart residential sector has experienced sustained growth over the past decade, driven by the convergence of IoT, IP connectivity, cloud services, and low-cost devices.

However, technological development has been primarily accompanied by:

- Communication standards.
- Automation platforms.
- Interoperability protocols.
- Technical integration frameworks.

**No structural commercial evaluation model** has been observed, either in academic literature or in the industrial market, that allows for the classification of domotics proposals from a perspective of risk, dependency, and systemic sustainability.

---

### 2.2 Technical Standards and Protocols

The industrial state of the art is dominated by technical standards such as:

- Zigbee
- Z-Wave
- Thread
- Matter
- KNX
- BACnet

These frameworks define:

- How devices communicate.
- How minimum levels of interoperability are ensured.
- How heterogeneous systems are integrated.

**However, these standards:**

- Do not evaluate the integrator's commercial model.
- Do not measure operational dependency.
- Do not classify structural sustainability.
- Do not differentiate between open architecture and captive ecosystems.

**Their focus is technical, not structural or strategic.**

---

### 2.3 Open Source Platforms and Ecosystems

Platforms such as:

- Home Assistant
- openHAB
- Domoticz

have contributed to the democratization of home control and integration.

These tools:

- Enable expanded interoperability.
- Reduce dependency on closed brands.
- Foster active technical communities.

**However, they do not constitute an evaluation framework.**  
They are technological infrastructures, not diagnostic models.

---

### 2.4 Academic Evaluation Approaches

Scientific literature contains research evaluating:

- IoT interoperability.
- Energy performance in smart homes.
- User interface usability.
- Middleware architectures.
- Multi-criteria systems for technology selection.

Some works utilize decision methodologies such as:

- SAW (Simple Additive Weighting)
- AHP (Analytic Hierarchy Process)
- Multi-criteria optimization models

These approaches are valuable for comparing specific technologies, but:

- They are not oriented toward the real market of integrators.
- They do not analyze commercial obsolescence risk.
- They do not consider geographic or regional dependency.
- They do not classify complete proposals as structural systems.

---

### 2.5 Identified Gap

The analysis of the state of the art reveals a **clear gap**:

**Extensive development exists in:**

- Protocols
- Technical architectures
- Middleware
- Platforms

**But no structural model exists that:**

- Evaluates complete domotics proposals.
- Classifies commercial architectural profiles.
- Measures provider dependency.
- Analyzes sustainability in regional contexts (e.g., LATAM).
- Enables objective comparison based on observable evidence.

Current market comparison is primarily conducted by:

- Price
- Brand
- Functional promise
- Marketing

**Not by structural architecture or systemic risk.**

---

### 2.6 DSEM Positioning

**DSEM (Domotics Structural Evaluation Model)** positions itself as:

>A typological and diagnostic framework oriented toward the structural evaluation of domotics proposals, independent of brand, technology, or scale.

**Its differential contribution lies in:**

- Multidimensional evaluation (infrastructure, dependency, sustainability).
- Non-hierarchical typological classification.
- Real commercial applicability.
- Consideration of regional context.
- Based on observable evidence, not provider declarations.

**The model does not compete with existing technical standards.**  
It operates at a higher layer: **the structural-strategic layer of the system.**

---

### 2.7 State of the Art Conclusion

Comparative analysis indicates that:

- **Existing standards** regulate communication.
- **Existing platforms** facilitate integration.
- **Academic literature** studies performance and architecture.
- **The market** commercializes closed or hybrid solutions.

**But there is no public, open, market-applicable structural model that classifies complete proposals according to risk, dependency, and sustainability.**

**DSEM is proposed to fill this gap.**

---

## 3. Research Problem

A review of the state of the art reveals a **lack of structured, public, and applicable frameworks** that simultaneously enable:

| Problem | Consequence |
|---------|-------------|
| Evaluate domotics architectures with verifiable technical criteria | Decisions based on marketing, not structure |
| Compare heterogeneous solutions under a single standard | Impossibility of objective tendering |
| Identify structural risks (lock-in, cloud dependency, obsolescence) | Orphaned systems, hidden costs |
| Translate technological architecture into understandable metrics for non-technical decision makers | Chronic information asymmetry |

Product certifications exist (Zigbee Compliance, KNX Certified) and electrical regulations (IEC 60364) are well established, but **none address the problem from the evaluator's perspective** — architect, developer, client — who must choose between radically different proposals.

The absence of such frameworks leads to suboptimal decisions and, in many cases, long-term technological dependencies that the contracting party discovers only when it is too late.

---

## 4. Model Objectives

DSEM aims to respond to the identified problems. Its objectives are:

| Objective | Description |
|----------|-------------|
| **O1** | Provide a structural evaluation framework based on observable evidence. |
| **O2** | Standardize comparative criteria between heterogeneous solutions. |
| **O3** | Introduce ordinal metrics (1-5) per dimension, replicable and auditable. |
| **O4** | Facilitate RFP, tendering, or technical analysis processes in professional environments. |
| **O5** | Promote architectural transparency as a differentiating value in the sector. |

The model does not seek to establish a universal hierarchy of "better domotics", but rather **to typify structural profiles** and allow the decision maker to consciously choose what level of risk they are willing to assume.

---

## 5. Methodology

DSEM defines **eight structural dimensions of analysis**. Each dimension is evaluated on an **ordinal scale from 1 to 5**, based exclusively on **observable evidence** (technical documentation, declared architecture, public specifications, verifiable responses in tender meetings).

### 5.1 Methodological Principles

1. **Observability:** Intentions, promises, and roadmaps are not evaluated. Only facts verifiable at the time of assessment.
2. **Ordinality:** The 1-5 scale reflects increasing degrees of structural maturity, not continuous scores.
3. **Modularity:** Dimensions are independent and can be weighted according to regional context or project typology.
4. **Openness:** The framework is public, modifiable, and evolutionary under the CC BY-SA 4.0 license.

---

### 5.2 Model Dimensions

#### D1 — Technological Infrastructure
*Type of architecture, use of open standards, declared interoperability.*

| Level | Observable Evidence |
|-------|---------------------|
| 1 | Only WiFi / Bluetooth retail devices, no central hub |
| 2 | Proprietary ecosystem with mandatory cloud |
| 3 | Physical hub but no declared standard |
| 4 | Explicit open standards (Zigbee, KNX, Modbus, MQTT, DALI) |
| 5 | Wired bus / documented distributed architecture |

**Detector question:** *"What protocols do you use, and what other brands can I connect?"*

---

#### D2 — Operational Dependency
*Level of functionality without connection to external servers or without the original provider.*

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
| 4 | Coordinated multi-system integration (e.g., blinds with temperature) |
| 5 | Energy management + conditional logic + historical monitoring |

**Detector question:** *"Give an example where two different systems talk to each other."*

---

#### D4 — Value Model
*Nature of the value offered (hardware, service, structural integration).*

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
*Technical level required for implementation and maintenance.*

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

**Detector question:** *Look at their website for 30 seconds. Do you see technology or just pretty photos?*

---

#### D7 — Ecosystem Sustainability
*Community, support, product lifecycle, spare parts availability.*

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
*User control over their data, server location, telemetry.*

| Level | Observable Evidence |
|-------|---------------------|
| 1 | Mandatory cloud, foreign servers, hidden telemetry |
| 2 | Mandatory cloud with regional servers |
| 3 | Hybrid: local + optional cloud |
| 4 | Local by default, cloud disableable |
| 5 | Local + open source / documented, zero telemetry |

**Detector question:** *"Does my data leave the country? Can you tell when I'm home?"*

---

## 6. Operational Structure

The DSEM model is not software or a closed platform. It is a **documented methodological framework** that includes:

| Tool | Function | Audience |
|------|---------|----------|
| **Architect's Checklist** | Ready-to-copy text for tender specifications | Prescribers |
| **Comparison Matrix** | Evaluation matrix with adjustable weighting | Technical evaluators |
| **Supplier Self-Assessment Form** | Sworn declaration for providers | Buyers |
| **Developer's Guide** | Translation of technical risk into resale value | Real estate developers |

All tools are **publicly accessible, modifiable, and evolutionary**, under the terms of the CC BY-SA 4.0 license.

---

## 7. Discussion

### 7.1 Conceptual Contribution

DSEM introduces a **paradigm shift** in the evaluation of home automation systems:

| Traditional Evaluation | DSEM Evaluation |
|-----------------------|-----------------|
| Brand-based | Architecture-based |
| Initial price-based | Structural risk-based |
| Functional promises-based | Observable evidence-based |
| Impossible comparison between ecosystems | Standardized typological comparison |

This shift enables the identification of:

- **Technological dependency risks** (vendor lock-in) that remain invisible in commercial evaluation.
- **Closed models disguised as open standards** (e.g., "we support Zigbee" but only with proprietary devices).
- **Architectures with low resilience** to internet outages, provider changes, or product discontinuation.
- **Sustainable ecosystems** versus **ephemeral solutions** with undeclared planned obsolescence.

### 7.2 Limitations

The model has limitations that must be explicitly acknowledged:

| Limitation | Implication |
|-----------|-------------|
| Dependence on declared or accessible information | Cannot evaluate what the provider deliberately hides |
| Residual subjectivity in score assignment | Requires minimum evaluator training |
| Does not evaluate information security or cybersecurity | Dimension deliberately excluded (requires specific framework) |
| Latin America-focused weighting (D2/D8) | Requires regional adaptation for other markets |

These limitations do not invalidate the model, but rather define its **perimeter of applicability** and guide its future development lines.

---

## 8. Implications for the Sector

The adoption of a framework like DSEM could have structural effects on the home automation market:

**1. Raising the technical standard in evaluation processes.**  
Tender specifications can demand concrete evidence instead of generic promises.

**2. Professionalization of decision-making.**  
Architects and developers can technically justify the selection of one provider over another.

**3. Reduction of information asymmetries.**  
The end client acquires a minimum vocabulary to ask about and understand what they are purchasing.

**4. Foundation for structural certifications.**  
DSEM can serve as the basis for an independent (non-commercial) technical seal.

---

## 9. Future Work

The model is published in version 1.0 as a **foundational document**. Planned development lines include:

| Line | Description | Status |
|------|-------------|--------|
| **Empirical validation** | Evaluation of 20 companies in the local market with publication of anonymized case studies | Pending |
| **Mathematical formalization** | Weighting system with adjustable parametric sensitivity | Pending |
| **Digital tool** | Interactive version of the comparison matrix (Web / Sheets) | In development |
| **Translation and regional adaptation** | Differentiated weightings for Europe, North America, Asia | Pending |
| **Integration with existing frameworks** | Cross-mapping with KNX, Zigbee, Matter certifications | Pending |

---

## 10. Conclusion

DSEM constitutes a **conceptual framework for evaluating home automation solutions from a structural and architectural perspective**, shifting the focus from marketing and superficial functionality toward sustainability, user sovereignty, and the technical maturity of the ecosystem.

In doing so, it contributes to:

- Professionalizing the relationship between providers and prescribers.
- Equipping the client with tools to ask questions and make decisions.
- Establishing a common language where fragmentation currently reigns.

Its **open, collaborative, and evolutionary nature** allows any sector actor — integrator, architect, developer, researcher — to use, critique, and improve it.

DSEM is not an endpoint.  
It is an **invitation to collectively build a standard where today there is only noise.**

---

## Acknowledgments

This model was built from direct experience in the **Argentine market**, where import restrictions, currency volatility, and scarcity of local technical support turn vendor lock-in into a structural, not theoretical, risk.

Inspired by:

- Open standards communities (Home Assistant, ESPHome, Tasmota, OpenHAB).
- Architects and developers tired of proprietary "black boxes".
- Clients who just wanted their home to work, not to be technological hostages.

---

## References

[1] KNX Association. *KNX Specifications – System Specifications*, 2024. URL: https://www.knx.org

[2] Connectivity Standards Alliance. *Matter Specification Version 1.3*, 2024. URL: https://csa-iot.org/all-solutions/matter/

[3] Zigbee Alliance. *Zigbee PRO Specification*, 2023. URL: https://csa-iot.org/all-solutions/zigbee/

[4] Home Assistant. *Open Source Home Automation Platform*, 2025. URL: https://www.home-assistant.io

[5] ESPHome. *ESPHome — Device Configuration for Home Automation*, 2025. URL: https://esphome.io

[6] Tasmota. *Tasmota — Open Source Firmware for ESP Devices*, 2025. URL: https://tasmota.github.io

[7] Saaty, T. L. *The Analytic Hierarchy Process: Planning, Priority Setting, Resource Allocation*. McGraw-Hill, 1980.

[8] Hwang, C. L. & Yoon, K. *Multiple Attribute Decision Making: Methods and Applications*. Springer-Verlag, 1981.

[9] Zanella, A. et al. *"Internet of Things for Smart Cities"*. IEEE Internet of Things Journal, Vol. 1, No. 1, pp. 22–32, 2014.

[10] Al-Fuqaha, A. et al. *"Internet of Things: A Survey on Enabling Technologies, Protocols, and Applications"*. IEEE Communications Surveys & Tutorials, Vol. 17, No. 4, pp. 2347–2376, 2015.

[11] Guinard, D. & Trifa, V. *Building the Web of Things*. Manning Publications, 2016.

[12] IRAM. *IRAM AEA 90364 – Reglamentación para instalaciones eléctricas en inmuebles*, 2021.

[13] IEC. *IEC 60364 – Low-voltage electrical installations*, 2020.

[14] Creative Commons. *CC BY-SA 4.0 License Legal Code*, 2025. URL: https://creativecommons.org/licenses/by-sa/4.0/legalcode

[15] OpenHAB Foundation. *openHAB – Empowering the Smart Home*, 2025. URL: https://www.openhab.org

[16] Domoticz. *Domoticz – Open Source Home Automation System*, 2025. URL: https://www.domoticz.com

[17] CENELEC. *EN 50090 – Home and Building Electronic Systems (HBES)*, 2022.

[18] ISO/IEC. *ISO/IEC 14543-3 – Information technology – Home electronic system (HES) architecture*, 2020.

[19] BSI. *BSI PAS 212 – Automated/proactive commissioning of IoT devices*, 2021.

[20] Mattern, F. & Floerkemeier, C. *"From the Internet of Computers to the Internet of Things"*. In: *Informatik-Spektrum*, Vol. 33, No. 2, pp. 107–121, 2010.

---

**Version 1.0 — March 2025**  
[github.com/cosolabs/dsem](https://github.com/cosolabs/dsem)  
**DOI:** *[Pending assignment]*

---

**License: CC BY-SA 4.0**  
Free use with attribution. Share improvements under same license. Commercial use allowed.
