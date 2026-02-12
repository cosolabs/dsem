# Análisis de Proveedor — DSEM v1.0

## 1. Case Metadata

| Field | Value |
|-------|-------|
| **Case ID** | `case-05.md` |
| **Title** | Integrador KNX con infraestructura cableada y estándar abierto |
| **Evaluator** | Anónimo |
| **Date** | 2026-02-12 |
| **Evidence source(s)** | Brochure residencial del proveedor |
| **Anonymization note** | Se han eliminado todas las marcas, nombres e identificadores del proveedor. Se preservan únicamente estándares tecnológicos. |

---

## 2. Provider / Proposal Summary

| Aspect | Description |
|--------|-------------|
| **Value proposition** | "Llave en mano", consultoría, diseño de proyectos, dirección de obra. Tecnología + diseño. KNX como estándar declarado. |
| **Business model** | Proyectos llave en mano. Consultoría + provisión + instalación + configuración. |
| **Target client** | Residencial premium, corporativo, hotelería, salud, estudios de arquitectura. |
| **Declared technology** | **KNX (estándar abierto, cableado bus)** . Integración de múltiples marcas del mercado. |

---

## 3. DSEM Dimensional Scoring

| Dimensión | Score (1-5) | Evidencia observable | Detector Question Answered |
|----------|-------------|---------------------|---------------------------|
| **D1 — Infraestructura** | **5/5** | "KNX, Estándar mundial para viviendas inteligentes, de topología mixta y con comunicación mediante un cable Bus (inmune a interferencias)". Declara explícitamente estándar abierto y cableado estructurado. | *What protocols? What other brands can I connect?* → **KNX. Cualquier marca certificada KNX.** |
| **D2 — Dependencia operativa** | **4/5** | "Control... tanto de forma local, como remota". No declara explícitamente funcionamiento sin internet, pero KNX por bus es 100% local por naturaleza. No hay documentación técnica pública visible. | *If you don't exist tomorrow, who fixes it?* → **Cualquier integrador KNX certificado. El estándar garantiza mantenibilidad por terceros.** |
| **D3 — Profundidad funcional** | **5/5** | Iluminación, cortinados/toldos, clima, riego, piscina/jacuzzi, multimedia multiroom, limpieza inteligente, red de datos, seguridad (3 niveles: disuasión, monitoreo, detección, reconocimiento facial, lectura de patentes, radar). Menciona lógica condicional: "sectorizando según humedad del suelo, clima, lluvia, tipo de plantas". | *Example where two systems talk to each other?* → **Sí. "Integrar luces y burbujas en una escena de iluminación del parque". Riego con sensores de humedad y clima. Seguridad con iluminación.** |
| **D4 — Modelo de valor** | **5/5** | "Trabajamos desde el formato 'llave en mano', acompañando todo el proceso de obra". "Consultoría, diseño de proyectos de corrientes débiles, su documentación y dirección de obra, provisión, instalación, configuración y puesta en marcha". | *How do you quote: per device, per hour, per project?* → **Por proyecto llave en mano con ingeniería a medida.** |
| **D5 — Complejidad estructural** | **5/5** | KNX con cableado bus. "Acompañando todo el proceso de obra". "Dirección de obra". "Documentación" de proyectos. Requiere planificación arquitectónica y tablero dedicado. | *At what stage of construction do you get involved?* → **Requiere planificación arquitectónica desde etapas tempranas de obra.** |
| **D6 — Transparencia tecnológica** | **4/5** | Declara **KNX explícitamente**. Menciona marcas específicas del mercado. Describe arquitectura de bus cableado. No publica esquemas ni topologías de red completas. | *Website: technology or just pretty photos?* → **Tecnología declarada con precisión. KNX, bus cableado, estándar abierto.** |
| **D7 — Sustentabilidad del ecosistema** | **5/5** | Basado en **KNX, estándar abierto internacional con más de 30 años de trayectoria**. Cualquier integrador certificado puede mantenerlo. Repuestos disponibles en el mercado global. No depende de la supervivencia del integrador. | *Where do I buy a spare part in 5 years?* → **Cualquier distribuidor KNX en el mundo. Estándar abierto garantizado.** |
| **D8 — Privacidad y soberanía de datos** | **2/5** | **No menciona absolutamente nada** sobre dónde se almacenan los datos, si usa nube, servidores, jurisdicción u opción local. El estándar KNX permite operación 100% local, pero el brochure no lo explicita. | *Does my data leave the country?* → **No declara. Sin información sobre privacidad ni soberanía de datos.** |

**Scoring criteria:** [DSEM Section 2](https://github.com/cosolabs/dsem?tab=readme-ov-file#2-the-8-structural-dimensions)

---

## 4. Context Weighting (Argentina / Latin America)

| Dimensión | Weight | Score | Weighted |
|----------|--------|-------|----------|
| D2 (Dependency) | 25% | 4 | 1.00 |
| D8 (Privacy) | 20% | 2 | 0.40 |
| D1 (Infrastructure) | 15% | 5 | 0.75 |
| D7 (Sustainability) | 15% | 5 | 0.75 |
| D3 (Functionality) | 10% | 5 | 0.50 |
| D6 (Transparency) | 8% | 4 | 0.32 |
| D5 (Complexity) | 5% | 5 | 0.25 |
| D4 (Value model) | 2% | 5 | 0.10 |
| **TOTAL** | **100%** | | **4.07 / 5** |

🔗 [DSEM Section 3 — Context Weighting](https://github.com/cosolabs/dsem?tab=readme-ov-file#3-context-weighting)

---

## 5. Structural Profile

| Profile | D1 | D2 | D7 | D8 | Score Range (/5) | Result |
|---------|-----|-----|-----|-----|------------------|--------|
| 🔴 Red — Ultra light | 1-2 | 1-2 | 1-2 | 1 | 1.00 - 1.75 | ❌ |
| 🟠 Orange — Heavy closed | 4-5 | 2-3 | 2-3 | 2-3 | 2.25 - 3.25 | ❌ |
| 🟢 Green — Open hybrid | 3-4 | 3-4 | 3-4 | 4 | 3.00 - 3.75 | ❌ |
| 🔵 Blue — Balanced architecture | 4 | 4-5 | 4-5 | 4-5 | 3.75 - 4.50 | ✅ |
| ⚫ Black — Critical infrastructure | 5 | 5 | 5 | 5 | 4.50 - 5.00 | ❌ |

**Determined profile:** 🔵 **Blue — Balanced architecture**  
**Descriptor:** *"Documentado, mantenible, estándares abiertos, infraestructura crítica."*

---

## 6. Summary of Structural Risks

| Risk Dimension | Observation |
|----------------|-------------|
| **Internet dependency** | **Bajo.** KNX por bus opera 100% local sin internet. El brochure menciona control local y remoto. |
| **Vendor lock-in** | **Nulo.** Estándar abierto KNX. Cualquier integrador certificado puede mantenerlo. |
| **Spare parts / repairability** | **Nulo.** Estándar internacional con más de 30 años. Repuestos garantizados en el mercado global. |
| **Data sovereignty** | **Crítico.** Nulo nivel de transparencia. No menciona dónde se almacenan los datos, si usa nube, servidores locales o híbridos. KNX permite operación local, pero el brochure no lo explicita. |
| **Documentation / transparency** | **Bajo.** Declara KNX y arquitectura de bus cableado. No publica esquemas ni topologías completas, pero el estándar está documentado públicamente. |
| **Functional limitations** | **Nulo.** Cobertura integral: iluminación, clima, riego, piscina, multimedia, limpieza, red, seguridad con reconocimiento facial y radar. |

---

## 7. Conclusion

**Este proveedor vende infraestructura domótica crítica basada en estándares abiertos.**

El perfil **🔵 Blue — Balanced architecture** indica que el cliente adquiere una **instalación técnica de grado profesional**, con:

- ✅ **Estándar abierto KNX:** Garantiza interoperabilidad, mantenibilidad por terceros y ciclo de vida >20 años.
- ✅ **Infraestructura cableada:** Bus KNX inmune a interferencias, sin dependencia de WiFi.
- ✅ **Sustentabilidad máxima:** Estándar internacional con respaldo global, no depende de la supervivencia del integrador.
- ✅ **Profundidad funcional total:** Integración de sistemas complejos con lógica condicional avanzada.
- ✅ **Modelo de ingeniería:** Proyecto llave en mano con documentación y dirección de obra.

**Debilidad crítica (única):**
- ❌ **Opacidad en privacidad y datos:** El brochure no menciona si las implementaciones usan nube, dónde se alojan los datos, ni ofrece políticas de privacidad. Tratándose de KNX, es técnicamente posible operar 100% local, pero el proveedor **no lo comunica**.

**Riesgo estructural: BAJO, con agravante en comunicación de privacidad.**  
Es el perfil más robusto de la muestra, con puntaje 4.07/5. Su única falla es no informar explícitamente sobre soberanía de datos, una carencia transversal a **todos los casos evaluados**.

---

## 8. Metadata

**License:** CC BY-SA 4.0  
**Attribution:** DSEM v1.0 — Matias Cacciagrano, 2025  
**Case study license:** Same as DSEM (open, share-alike)

*This case is an anonymized contribution to the DSEM open standard.*

🔗 [github.com/cosolabs/dsem](https://github.com/cosolabs/dsem)
