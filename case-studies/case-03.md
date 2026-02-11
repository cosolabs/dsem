# Análisis de Proveedor — DSEM v1.0

## 1. Case Metadata

| Field | Value |
|-------|-------|
| **Case ID** | `case-03.md` |
| **Title** | Proveedor de domótica con app propietaria y operación manual offline |
| **Evaluator** | Anónimo |
| **Date** | 2026-02-11 |
| **Evidence source(s)** | Sitio web del proveedor |
| **Anonymization note** | Se ha preservado el nombre del proveedor como parte del caso de estudio público. |

---

## 2. Provider / Proposal Summary

| Aspect | Description |
|--------|-------------|
| **Value proposition** | "App creada y desarrollada por nosotros, fácil, intuitiva y autoconfigurable. Totalmente gratuita y sin límite en cantidad de dispositivos." |
| **Business model** | Venta de dispositivos + instalación por técnicos propios. Sin abono mensual. |
| **Target client** | Residencial (casas y departamentos), tanto obra nueva como terminada. Edificios completos. |
| **Declared technology** | **App propietaria.** Compatible con asistentes Amazon Alexa y Google Home. **No declara protocolos** (Zigbee, WiFi, KNX, MQTT, etc.). |

---

## 3. DSEM Dimensional Scoring

| Dimensión | Score (1-5) | Evidencia observable | Detector Question Answered |
|----------|-------------|---------------------|---------------------------|
| **D1 — Infraestructura** | **1/5** | No declara protocolos. Menciona "dispositivos" pero no especifica si son WiFi, Zigbee u otro. No menciona hub físico ni arquitectura cableada. | *What protocols? What other brands can I connect?* → **No declara. Solo dispositivos de su marca.** |
| **D2 — Dependencia operativa** | **1/5** | **No hay funcionamiento inteligente sin internet.** La pregunta "¿Qué pasa si me quedo sin internet?" responde: "Vas a poder controlar tu casa **manualmente de manera convencional**." No hay operación offline vía app. | *If you don't exist tomorrow, who fixes it?* → **No hay evidencia de documentación técnica para terceros.** |
| **D3 — Profundidad funcional** | **2/5** | Iluminación, climatización (AA, termostatos, ventiladores), cortinas/persianas/toldos, TV/audio, escenas, compatibilidad con asistentes. **No menciona seguridad (cámaras, alarmas), gestión energética ni lógica condicional avanzada.** | *Example where two systems talk to each other?* → **Escenas programadas (varios dispositivos). No se evidencia lógica cruzada condicional compleja.** |
| **D4 — Modelo de valor** | **2/5** | "Nuestros técnicos se encargan de realizar la instalación y programación." Venta de dispositivos + instalación. Sin costo de app. | *How do you quote: per device, per hour, per project?* → **Esquema de dispositivo + instalación.** |
| **D5 — Complejidad estructural** | **2/5** | Instalación en casas terminadas y en construcción. "Puede instalarse en casas, departamentos o en hasta un edificio completo." **No menciona si requiere cableado, obras o tablero dedicado.** | *At what stage of construction do you get involved?* → **Ambos: obra nueva y retrofit.** |
| **D6 — Transparencia tecnológica** | **1/5** | **Marketing puro.** El sitio muestra capturas de app, íconos y descripciones funcionales. **No menciona protocolos, frecuencias, marcas de hardware, topología ni arquitectura de red.** | *Website: technology or just pretty photos?* → **Solo descripciones funcionales y marketing. Cero transparencia tecnológica.** |
| **D7 — Sustentabilidad del ecosistema** | **1/5** | No informa sobre repuestos a futuro. Ecosistema cerrado. Dependencia total de una sola marca. | *Where do I buy a spare part in 5 years?* → **No responde. Sin garantía de repuestos.** |
| **D8 — Privacidad y soberanía de datos** | **1/5** | **No menciona absolutamente nada** sobre dónde se almacenan los datos, si usa nube, servidores, jurisdicción o si hay opción local. La app requiere internet para control remoto. | *Does my data leave the country?* → **No declara. Sin información sobre privacidad ni soberanía de datos.** |

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
| D5 (Complexity) | 5% | 2 | 0.10 |
| D4 (Value model) | 2% | 2 | 0.04 |
| **TOTAL** | **100%** | | **1.17 / 5** |

🔗 [DSEM Section 3 — Context Weighting](https://github.com/cosolabs/dsem?tab=readme-ov-file#3-context-weighting)

---

## 5. Structural Profile

| Profile | D1 | D2 | D7 | D8 | Score Range (/5) | Descriptor |
|---------|-----|-----|-----|-----|------------------|------------|
| 🔴 **Red — Ultra light** | 1-2 | 1-2 | 1-2 | 1 | **1.00 - 1.75** | Gadgets, nube obligatoria, descartables |
| 🟠 **Orange — Heavy closed** | 4-5 | 2-3 | 2-3 | 2-3 | **2.25 - 3.25** | Profesional pero cautivo |
| 🟢 **Green — Open hybrid** | 3-4 | 3-4 | 3-4 | 4 | **3.00 - 3.75** | Hardware commodity + local |
| 🔵 **Blue — Balanced architecture** | 4 | 4-5 | 4-5 | 4-5 | **3.75 - 4.50** | Documentado, mantenible |
| ⚫ **Black — Critical infrastructure** | 5 | 5 | 5 | 5 | **4.50 - 5.00** | Grado industrial/hospital |

**Determined profile:** 🔴 **Red — Ultra light**  
**Descriptor:** *"Gadgets, nube obligatoria, descartables."*

🔗 [DSEM Section 4 — Structural Profiles](https://github.com/cosolabs/dsem?tab=readme-ov-file#4-structural-profiles)

---

## 6. Summary of Structural Risks

| Risk Dimension | Observation |
|----------------|-------------|
| **Internet dependency** | **Crítico.** Sin internet, **no hay control por app ni automatización**. Solo operación manual convencional. El proveedor no menciona funcionamiento offline inteligente. |
| **Vendor lock-in** | **Crítico.** Ecosistema cerrado. No declara protocolos ni admite otras marcas. |
| **Spare parts / repairability** | **Crítico.** No informa repuestos a futuro. Dependencia total de una marca sin garantía de continuidad. |
| **Data sovereignty** | **Crítico.** **Nulo nivel de transparencia.** No menciona dónde se almacenan los datos, si usa nube, servidores ni jurisdicción. |
| **Documentation / transparency** | **Crítico.** Solo marketing funcional. No hay documentación técnica pública. Imposible mantenimiento por terceros. |
| **Functional limitations** | **Moderado.** Cubre iluminación, climatización básica, cortinados y audio. **Sin seguridad, gestión energética ni lógica condicional avanzada.** |

---

## 7. Conclusion

**Este proveedor vende un ecosistema cerrado de gadgets, no infraestructura domótica abierta y sustentable.**

El perfil **🔴 Ultra light** es contundente: el cliente no adquiere una instalación técnica, sino una **dependencia comercial y tecnológica**.

**Agravantes críticos específicos de este caso:**

1. **Nula operación offline inteligente:** A diferencia de otros casos ultra light que al menos permiten control local vía app, **reduce el hogar a operación manual convencional** cuando no hay internet. No hay domótica sin conexión.

2. **Opacidad tecnológica total:** El sitio no menciona **ningún** protocolo, estándar, frecuencia o arquitectura. Es el caso con menor transparencia tecnológica entre los evaluados.

3. **Silencio absoluto sobre datos:** Es el único caso que **ni siquiera menciona la existencia de una nube**. El cliente no tiene forma de saber si sus datos existen, dónde están o quién los accede.

**Riesgo estructural: MÁXIMO.**  
El perfil es Ultra light con **agravantes de nula operación offline, opacidad total y ecosistema 100% cautivo**. Si el proveedor desaparece, el cliente pierde **toda** la funcionalidad inteligente y queda con hardware huérfano.

---

## 8. Metadata

**License:** CC BY-SA 4.0  
**Attribution:** DSEM v1.0 — Matias Cacciagrano, 2025  
**Case study license:** Same as DSEM (open, share-alike)

*This case is a public contribution to the DSEM open standard.*

🔗 [github.com/cosolabs/dsem](https://github.com/cosolabs/dsem)
