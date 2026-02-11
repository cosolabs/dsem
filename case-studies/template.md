# DSEM Case Study Template

Use this template to document your own structural evaluations.  
All fields marked with `[ ]` must be completed with observable evidence.

🔗 **DSEM v1.0 — Domotics Structural Evaluation Model**  
📘 [github.com/cosolabs/dsem](https://github.com/cosolabs/dsem)

---

## 1. Case Metadata

| Field | Value |
|-------|-------|
| **Case ID** | `case-XX.md` |
| **Title** | [Brief, anonymous description] |
| **Evaluator** | [Name or handle / Anonymous] |
| **Date** | [YYYY-MM-DD] |
| **Evidence source(s)** | [Website URL, brochure, meeting notes, proposal document] |
| **Anonymization note** | [All brands, names and identifiers have been removed] |

---

## 2. Provider / Proposal Summary

| Aspect | Description |
|--------|-------------|
| **Value proposition** | [What do they promise? "Sin obras", "AI", "eco", etc.] |
| **Business model** | [Device sale, installation, subscription, turnkey] |
| **Target client** | [Residential, commercial, new build, retrofit] |
| **Declared technology** | [WiFi, Zigbee, KNX, proprietary, etc. — or "none declared"] |

---

## 3. DSEM Dimensional Scoring

| Dimension | Score (1-5) | Observable Evidence | Detector Question Answered |
|----------|-------------|---------------------|---------------------------|
| **D1 — Infrastructure** |  |  | *What protocols? What other brands can I connect?* |
| **D2 — Operational dependency** |  |  | *If you don't exist tomorrow, who fixes it?* |
| **D3 — Functional depth** |  |  | *Example where two systems talk to each other?* |
| **D4 — Value model** |  |  | *How do you quote: per device, per hour, per project?* |
| **D5 — Structural complexity** |  |  | *At what stage of construction do you get involved?* |
| **D6 — Technological transparency** |  |  | *Website: technology or just pretty photos?* |
| **D7 — Ecosystem sustainability** |  |  | *Where do I buy a spare part in 5 years?* |
| **D8 — Privacy and data sovereignty** |  |  | *Does my data leave the country?* |

**Scoring criteria:** [DSEM Section 2](https://github.com/cosolabs/dsem?tab=readme-ov-file#2-the-8-structural-dimensions)

---

## 4. Context Weighting (Argentina / Latin America)

| Dimension | Weight | Score | Weighted |
|----------|--------|-------|----------|
| D2 (Dependency) | 25% |  |  |
| D8 (Privacy) | 20% |  |  |
| D1 (Infrastructure) | 15% |  |  |
| D7 (Sustainability) | 15% |  |  |
| D3 (Functionality) | 10% |  |  |
| D6 (Transparency) | 8% |  |  |
| D5 (Complexity) | 5% |  |  |
| D4 (Value model) | 2% |  |  |
| **TOTAL** | **100%** | | **/100** |

🔗 [DSEM Section 3 — Context Weighting](https://github.com/cosolabs/dsem?tab=readme-ov-file#3-context-weighting)

---

## 5. Structural Profile

| Profile | D1 | D2 | D7 | D8 | Score Range | Result |
|---------|-----|-----|-----|-----|-------------|--------|
| 🔴 Red — Ultra light | 1-2 | 1-2 | 1-2 | 1 | 20-35 | |
| 🟠 Orange — Heavy closed | 4-5 | 2-3 | 2-3 | 2-3 | 45-65 | |
| 🟢 Green — Open hybrid | 3-4 | 3-4 | 3-4 | 4 | 60-75 | |
| 🔵 Blue — Balanced architecture | 4 | 4-5 | 4-5 | 4-5 | 75-90 | |
| ⚫ Black — Critical infrastructure | 5 | 5 | 5 | 5 | 90-100 | |

**Determined profile:** [ ]  
🔗 [DSEM Section 4 — Structural Profiles](https://github.com/cosolabs/dsem?tab=readme-ov-file#4-structural-profiles)

---

## 6. Summary of Structural Risks

| Risk Dimension | Observation |
|----------------|-------------|
| **Internet dependency** | [ ] |
| **Vendor lock-in** | [ ] |
| **Spare parts / repairability** | [ ] |
| **Data sovereignty** | [ ] |
| **Documentation / transparency** | [ ] |
| **Functional limitations** | [ ] |

---

## 7. Conclusion

[Brief, factual summary. What does this profile mean for the client?]

---

## 8. Metadata

**License:** CC BY-SA 4.0  
**Attribution:** DSEM v1.0 — Matias Cacciagrano, 2025  
**Case study license:** Same as DSEM (open, share-alike)

*This case is an anonymized contribution to the DSEM open standard.*
