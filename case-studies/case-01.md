# Análisis de Proveedor — DSEM v1.0

## 1. Case Metadata

| Field | Value |
|-------|-------|
| **Case ID** | `case-01.md` |
| **Title** | Proveedor de domótica WiFi con dependencia total de nube |
| **Evaluator** | Anónimo |
| **Date** | 2026-02-11 |
| **Evidence source(s)** | Sitio web del proveedor (publicado 2020) |
| **Anonymization note** | Se han eliminado todas las marcas, nombres e identificadores del proveedor. |

---

## 2. Provider / Proposal Summary

| Aspect | Description |
|--------|-------------|
| **Value proposition** | "Sin obras", control desde el celular, "hogar inteligente", familias felices. |
| **Business model** | Venta por dispositivo + instalación. No hay ingeniería a medida ni infraestructura. |
| **Target client** | Residencial, principalmente casas ya construidas (retrofit). |
| **Declared technology** | Solo WiFi. No declara estándares abiertos (Zigbee, KNX, MQTT). |

---

## 3. DSEM Dimensional Scoring

| Dimensión | Score (1-5) | Evidencia observable | Detector Question Answered |
|----------|-------------|---------------------|---------------------------|
| **D1 — Infraestructura** | 1/5 | Solo WiFi. "Sin obras". No declara estándares abiertos (Zigbee, KNX, MQTT). | *What protocols? What other brands can I connect?* → **Solo WiFi propietario. No admite otras marcas.** |
| **D2 — Dependencia operativa** | 1/5 | No menciona funcionamiento offline. No entrega documentación técnica. Sistema no rescatable si la empresa desaparece. | *If you don't exist tomorrow, who fixes it?* → **Nadie. El sistema muere sin su nube.** |
| **D3 — Profundidad funcional** | 2/5 | Luces, cerraduras, aire, timbre, seguridad básica. Sin integración HVAC real, gestión energética ni lógica condicional avanzada. | *Example where two systems talk to each other?* → **No se evidencia.** |
| **D4 — Modelo de valor** | 1/5 | Venta por dispositivo + instalación. No hay ingeniería a medida ni infraestructura. | *How do you quote: per device, per hour, per project?* → **Por dispositivo + instalación.** |
| **D5 — Complejidad estructural** | 1/5 | "Sin obras" = Plug & Play. No requiere plano, etapa de construcción ni tablero dedicado. | *At what stage of construction do you get involved?* → **Solo retrofit, sin planificación.** |
| **D6 — Transparencia tecnológica** | 1/5 | Solo marketing: familias felices, ambientes lindos, frases genéricas. No menciona protocolos, marcas ni arquitectura. | *Website: technology or just pretty photos?* → **Solo fotos y frases aspiracionales.** |
| **D7 — Sustentabilidad del ecosistema** | 1/5 | No informa repuestos a futuro. Dependencia de marca no declarada. Perfil: hardware discontinuado en <2 años. | *Where do I buy a spare part in 5 years?* → **No responde. Sin garantía de repuestos.** |
| **D8 — Privacidad y soberanía de datos** | 1/5 | No informa dónde se almacenan los datos. No ofrece opción local. Nube obligatoria, servidores no declarados. | *Does my data leave the country?* → **No declara. Nube obligatoria, servidores desconocidos.** |

**Scoring criteria:** [DSEM Section 2](https://github.com/cosolabs/dsem?tab=readme-ov-file#2-the-8-structural-dimensions)

---

## 4. Context Weighting (Argentina / Latin America)

| Dimensión | Weight | Score | Weighted |
|----------|--------|-------|----------|
| D2 (Dependency) | 25% | 1 | 0.25 |
| D8 (Privacy) | 20% | 1 | 0.20 |
| D1 (Infrastructure) | 15% | 1 | 0.15 |
| D7 (Sustainability) | 15% | 1 | 0.15 |
| D3 (Functionality) | 10% | 2 | 0.20 |
| D6 (Transparency) | 8% | 1 | 0.08 |
| D5 (Complexity) | 5% | 1 | 0.05 |
| D4 (Value model) | 2% | 1 | 0.02 |
| **TOTAL** | **100%** | | **1.10 / 5** |

🔗 [DSEM Section 3 — Context Weighting](https://github.com/cosolabs/dsem?tab=readme-ov-file#3-context-weighting)

---

## 5. Structural Profile

| Profile | D1 | D2 | D7 | D8 | Score Range | Result |
|---------|-----|-----|-----|-----|-------------|--------|
| 🔴 Red — Ultra light | 1-2 | 1-2 | 1-2 | 1 | 20-35 | ✅ |
| 🟠 Orange — Heavy closed | 4-5 | 2-3 | 2-3 | 2-3 | 45-65 | ❌ |
| 🟢 Green — Open hybrid | 3-4 | 3-4 | 3-4 | 4 | 60-75 | ❌ |
| 🔵 Blue — Balanced architecture | 4 | 4-5 | 4-5 | 4-5 | 75-90 | ❌ |
| ⚫ Black — Critical infrastructure | 5 | 5 | 5 | 5 | 90-100 | ❌ |

**Determined profile:** 🔴 **Red — Ultra light**  
**Descriptor:** *"Gadgets, nube obligatoria, descartables."*

🔗 [DSEM Section 4 — Structural Profiles](https://github.com/cosolabs/dsem?tab=readme-ov-file#4-structural-profiles)

---

## 6. Summary of Structural Risks

| Risk Dimension | Observation |
|----------------|-------------|
| **Internet dependency** | **Crítico.** No menciona funcionamiento offline. Sistema inoperable sin conexión a nube. |
| **Vendor lock-in** | **Crítico.** Solo WiFi propietario. Sin estándares abiertos. Imposible integrar equipos de terceros. |
| **Spare parts / repairability** | **Crítico.** No informa repuestos a futuro. Hardware con perfil de electrónica de consumo, discontinuable en <2 años. |
| **Data sovereignty** | **Crítico.** Nube obligatoria. No declara servidores ni jurisdicción. Datos personales sin soberanía. |
| **Documentation / transparency** | **Crítico.** Solo manuales de usuario. No hay documentación técnica para mantenimiento de terceros. |
| **Functional limitations** | **Moderado.** Luces, cerraduras, seguridad básica. Sin integración HVAC real, gestión energética ni lógica condicional avanzada. |

---

## 7. Conclusion

**Este proveedor vende gadgets, no infraestructura domótica abierta y sustentable.**

El perfil **🔴 Ultra light** indica que el cliente no adquiere una instalación técnica, sino una **dependencia comercial y tecnológica**. El sistema depende absolutamente de la nube del proveedor, no tiene estándares abiertos, no garantiza repuestos y opera sin transparencia sobre el destino de los datos.

**Riesgo estructural: MÁXIMO.**  
El cliente queda cautivo de un ecosistema cerrado sin posibilidad de migración, mantenimiento por terceros ni soberanía de datos. Si el proveedor desaparece o discontinuúa la línea, el sistema queda obsoleto sin solución.

---

## 8. Metadata

**License:** CC BY-SA 4.0  
**Attribution:** DSEM v1.0 — Matias Cacciagrano, 2025  
**Case study license:** Same as DSEM (open, share-alike)

*This case is an anonymized contribution to the DSEM open standard.*

🔗 [github.com/cosolabs/dsem](https://github.com/cosolabs/dsem)
