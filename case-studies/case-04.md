# Análisis de Proveedor — DSEM v1.0

## 1. Case Metadata

| Field | Value |
|-------|-------|
| **Case ID** | `case-04.md` |
| **Title** | Integrador de marcas premium con foco en entretenimiento y confort |
| **Evaluator** | Anónimo |
| **Date** | 2026-02-11 |
| **Evidence source(s)** | Sitio web del proveedor |
| **Anonymization note** | Se ha preservado el nombre del proveedor como parte del caso de estudio público. |

---

## 2. Provider / Proposal Summary

| Aspect | Description |
|--------|-------------|
| **Value proposition** | "Especialistas diseñando e instalando proyectos tecnológicos, integrando las principales marcas." Showroom físico. Foco en experiencia, diseño, confort y entretenimiento. |
| **Business model** | Diseño e instalación de proyectos tecnológicos. Integración de marcas premium. No hay mención a costos de mantenimiento ni suscripciones. |
| **Target client** | Residencial de alto perfil. Menciona "familias ocupadas", "estilos de vida", "diseño de interiores". Presencia en Nordelta (segmento ABC1). |
| **Declared technology** | **Integración de marcas:** Control4, Lutron, Crestron. Protocolos no declarados explícitamente, pero las marcas mencionadas operan sobre Zigbee, RF, cableado estructurado y sistemas propietarios profesionales. |

---

## 3. DSEM Dimensional Scoring

| Dimensión | Score (1-5) | Evidencia observable | Detector Question Answered |
|----------|-------------|---------------------|---------------------------|
| **D1 — Infraestructura** | **4/5** | Integra **marcas profesionales** (Control4, Lutron, Crestron). No declara explícitamente protocolos abiertos, pero estas marcas trabajan con estándares de la industria (Zigbee, RF, cableado). Menciona "sensores inteligentes", "dimmers", "motorización". | *What protocols? What other brands can I connect?* → **Control4, Lutron, Crestron. Ecosistema abierto a integración de múltiples marcas premium.** |
| **D2 — Dependencia operativa** | **3/5** | No menciona explícitamente funcionamiento offline. Sin embargo, los sistemas profesionales (Crestron, Lutron, Control4) **soportan operación local** por diseño. No hay evidencia de documentación técnica pública para terceros. | *If you don't exist tomorrow, who fixes it?* → **Otro integrador puede tomar el sistema si conoce las plataformas. Dependencia de las marcas, no del integrador.** |
| **D3 — Profundidad funcional** | **4/5** | Control de climatización, iluminación, seguridad (alarmas, cámaras, accesos), cortinados/persianas, audio multiroom, video distribuido, cine en casa, intercom, WiFi. Menciona **escenas y lógica condicional**: "si el sol ya no ilumina el living, ajustar temperatura, cerrar persianas, adecuar iluminación". | *Example where two systems talk to each other?* → **Sí. Iluminación + climatización + persianas coordinados. Seguridad + iluminación programada para simular presencia.** |
| **D4 — Modelo de valor** | **4/5** | "Diseñando e instalando proyectos tecnológicos". No venden dispositivos sueltos sino **soluciones integrales**. Enfoque en ingeniería de proyecto y programación a medida. | *How do you quote: per device, per hour, per project?* → **Por proyecto con ingeniería a medida.** |
| **D5 — Complejidad estructural** | **4/5** | Menciona "planeamiento", "programación", "diseño de interiores y exteriores". Integración con arquitectura. No especifica si requieren obra o cableado, pero por las marcas (Crestron, Lutron) **implican infraestructura dedicada**. | *At what stage of construction do you get involved?* → **Requieren planificación arquitectónica. Perfil de instalación profesional.** |
| **D6 — Transparencia tecnológica** | **3/5** | Menciona **marcas concretas** (Control4, Lutron, Crestron). Describe funcionalidades con precisión. **No publica esquemas, topologías ni arquitectura de red.** Marketing aspiracional pero con sustento técnico. | *Website: technology or just pretty photos?* → **Mixto. Fotos de ambientes, pero también descripciones técnicas y marcas declaradas.** |
| **D7 — Sustentabilidad del ecosistema** | **4/5** | Basado en **marcas establecidas** (Lutron: 60+ años, Crestron: 50+ años, Control4: 20+ años). Ecosistema con respaldo internacional, red de integradores y repuestos disponibles. El hardware profesional tiene ciclo de vida >10 años. | *Where do I buy a spare part in 5 years?* → **A través de cualquier integrador oficial de esas marcas. No depende de la marca.** |
| **D8 — Privacidad y soberanía de datos** | **2/5** | **No menciona absolutamente nada** sobre datos, nube, servidores ni privacidad. Los sistemas profesionales pueden operar 100% locales, pero el sitio no informa si sus implementaciones usan nube ni dónde se alojan los datos. | *Does my data leave the country?* → **No declara. No hay política de privacidad visible en el sitio.** |

**Scoring criteria:** [DSEM Section 2](https://github.com/cosolabs/dsem?tab=readme-ov-file#2-the-8-structural-dimensions)

---

## 4. Context Weighting (Argentina / Latin America)

| Dimensión | Weight | Score | Weighted |
|----------|--------|-------|----------|
| D2 (Dependency) | 25% | 3 | 0.75 |
| D8 (Privacy) | 20% | 2 | 0.40 |
| D1 (Infrastructure) | 15% | 4 | 0.60 |
| D7 (Sustainability) | 15% | 4 | 0.60 |
| D3 (Functionality) | 10% | 4 | 0.40 |
| D6 (Transparency) | 8% | 3 | 0.24 |
| D5 (Complexity) | 5% | 4 | 0.20 |
| D4 (Value model) | 2% | 4 | 0.08 |
| **TOTAL** | **100%** | | **3.27 / 5** |

🔗 [DSEM Section 3 — Context Weighting](https://github.com/cosolabs/dsem?tab=readme-ov-file#3-context-weighting)

---

## 5. Structural Profile (Escala /5)

| Profile | D1 | D2 | D7 | D8 | Score Range (/5) | Result |
|---------|-----|-----|-----|-----|------------------|--------|
| 🔴 Red — Ultra light | 1-2 | 1-2 | 1-2 | 1 | 1.00 - 1.75 | ❌ |
| 🟠 Orange — Heavy closed | 4-5 | 2-3 | 2-3 | 2-3 | 2.25 - 3.25 | ❌ |
| 🟢 Green — Open hybrid | 3-4 | 3-4 | 3-4 | 4 | 3.00 - 3.75 | ❌ |
| 🔵 **Blue — Balanced architecture** | 4 | 4-5 | 4-5 | 4-5 | **3.75 - 4.50** | ✅ |
| ⚫ Black — Critical infrastructure | 5 | 5 | 5 | 5 | 4.50 - 5.00 | ❌ |

**Determined profile:** 🔵 **Blue — Balanced architecture**  
**Descriptor:** *"Documentado, mantenible, estándares abiertos en la práctica, pero con opacidad en datos."*

🔗 [DSEM Section 4 — Structural Profiles](https://github.com/cosolabs/dsem?tab=readme-ov-file#4-structural-profiles)

---

## 6. Summary of Structural Risks

| Risk Dimension | Observation |
|----------------|-------------|
| **Internet dependency** | **No declarado.** Por las marcas que integran, es altamente probable que soporten operación local, pero el sitio no lo explicita. |
| **Vendor lock-in** | **Bajo.** El lock-in es hacia las marcas (Control4, Lutron, Crestron), no hacia el integrador. Existen múltiples integradores certificados para esas plataformas. |
| **Spare parts / repairability** | **Bajo.** Marcas con décadas de trayectoria, canales de repuestos establecidos y ciclos de vida largos. |
| **Data sovereignty** | **Crítico.** **Nulo nivel de transparencia.** El sitio no menciona dónde se almacenan los datos, si los sistemas implementados usan nube, servidores locales o híbridos. Es el punto más débil. |
| **Documentation / transparency** | **Moderado.** Declaran marcas y funcionalidades con precisión. No publican documentación técnica ni arquitecturas. |
| **Functional limitations** | **Bajo.** Cobertura completa: climatización, iluminación, seguridad, cortinados, audio, video, intercom, escenas complejas con lógica condicional. |

---

## 7. Conclusion

**Este proveedor vende infraestructura domótica profesional, no gadgets.**

El perfil **🔵 Blue — Balanced architecture** indica que el cliente adquiere una **instalación técnica basada en estándares de la industria**, con marcas de larga trayectoria, soporte internacional y posibilidad de ser mantenida por otros integradores.

**Fortalezas estructurales:**
- ✅ **Infraestructura sólida:** Basada en marcas profesionales (Lutron, Crestron, Control4).
- ✅ **Sustentabilidad garantizada:** Ecosistemas con décadas de respaldo y repuestos asegurados.
- ✅ **Profundidad funcional real:** Lógica condicional, escenas coordinadas, integración multisistema.
- ✅ **Modelo de ingeniería:** Cotización por proyecto, no por dispositivo.

**Debilidad crítica:**
- ❌ **Opacidad total en privacidad y datos:** El sitio no menciona si sus sistemas operan 100% locales, si usan nube, dónde se alojan los datos, ni ofrece políticas de privacidad. En un contexto Latam con peso del 20% en D8, esta falta de transparencia penaliza fuertemente el puntaje.

**Riesgo estructural: MODERADO, con agravante en soberanía de datos.**  
El cliente obtiene un sistema profesional, mantenible y sustentable, pero **desconoce completamente el destino de sus datos**. Para un perfil ABC1 con preocupaciones de seguridad y privacidad, esta opacidad es inconsistente con el posicionamiento premium.

---

## 8. Metadata

**License:** CC BY-SA 4.0  
**Attribution:** DSEM v1.0 — Matias Cacciagrano, 2025  
**Case study license:** Same as DSEM (open, share-alike)

*This case is a public contribution to the DSEM open standard.*

🔗 [github.com/cosolabs/dsem](https://github.com/cosolabs/dsem)
