# Análisis de Proveedor — DSEM v1.0

## 1. Case Metadata

| Field | Value |
| :--- | :--- |
| **Case ID** | case-06.md |
| **Title** | Integrador especialista en documentación técnica y reparación de sistemas huérfanos |
| **Evaluator** | Anónimo |
| **Date** | 2026-02-17 |
| **Evidence source(s)** | Sitio web del proveedor: Secciones "Nosotros", "Servicios", "Trabajos Realizados", Post del blog "La eterna pelea por la Documentación". |
| **Anonymization note** | Se ha preservado el nombre del proveedor como parte del caso de estudio público, siguiendo el formato de los casos 01-04. |

## 2. Provider / Proposal Summary

| Aspect | Description |
| :--- | :--- |
| **Value proposition** | Soluciones completas de automatización, integración y tecnología para viviendas y espacios empresariales, incluyendo diseño, instalación, redes, AV y sistemas de control integrados. Énfasis en la **documentación técnica** como pilar fundamental del proyecto. |
| **Business model** | Proyectos a medida + instalación + soporte técnico. Línea destacada de servicios "revivir instalaciones" de terceros que carecen de documentación. |
| **Target client** | Residencial alto estándar y espacios comerciales que buscan integración tecnológica integral. Especialmente atractivo para propietarios con instalaciones existentes problemáticas. |
| **Declared technology** | Integración de múltiples tecnologías (seguridad electrónica, redes de datos cableadas, audio y video distribuidos). En servicios de reparación, aplican normas CEDIA y AVIXA para identificación y documentación. No se detalla arquitectura abierta estándar en la web pública. |

## 3. DSEM Dimensional Scoring

| Dimensión | Score (1-5) | Evidencia observable | Detector Question Answered |
| :--- | :--- | :--- | :--- |
| **D1 — Infraestructura** | **3/5** | Ofrece diseño técnico y redes cableadas. No declara protocolos abiertos (KNX, MQTT, DALI). Su fortaleza es metodológica (documentación CEDIA/AVIXA), no la promesa de interoperabilidad por estándares declarados. | **What protocols? What other brands can I connect?** → No se especifican protocolos abiertos. La interoperabilidad futura depende de la calidad de la documentación, no de un estándar declarado. |
| **D2 — Dependencia operativa** | **3/5** | Filosofía de "la documentación es del cliente" explícita en blog. Entregan planos y documentación. En la práctica, ¿es suficiente para que otro integrador opere sin ellos? No hay evidencia pública del nivel de detalle. Riesgo moderado. | **If you don't exist tomorrow, who fixes it?** → En teoría, cualquier integrador competente gracias a la documentación. En la práctica, el nivel de detalle documentado es una incógnita pública. |
| **D3 — Profundidad funcional** | **4/5** | Integración de iluminación, seguridad, audio, video y redes en proyectos complejos. Evidencia de soluciones integrales con diseño detallado. | **Example where two systems talk to each other?** → Sí, integración de múltiples sistemas en un proyecto unificado (iluminación + seguridad + AV). |
| **D4 — Modelo de valor** | **4/5** | Venden ingeniería y conocimiento. Postura clara en blog: el cliente paga por documentación y planificación para garantizar calidad y vida útil. Modelo profesional por proyecto, no por dispositivo. | **How do you quote: per device, per hour, or per project?** → Por proyecto, con ingeniería a medida. La documentación es un entregable clave. |
| **D5 — Complejidad estructural** | **4/5** | Participa en etapas de obra, diseño de racks y cableado estructurado. Perfil de instalación profesional que requiere planificación arquitectónica. | **At what stage of construction do you get involved?** → Requiere planificación arquitectónica para proyectos nuevos. En reparaciones, intervienen en cualquier etapa post-construcción. |
| **D6 — Transparencia tecnológica** | **3/5** | El sitio muestra credenciales, membresías (CEDIA/AVIXA) y contenido conceptual sobre documentación. No publica esquemas, topologías ni arquitecturas concretas. | **Website: technology or just pretty photos?** → Mixto. Hay evidencia de filosofía de trabajo y metodología, pero poca profundidad técnica pública. |
| **D7 — Sustentabilidad del ecosistema** | **3/5** | Utiliza marcas reconocidas del mercado (por sus credenciales), lo que facilita repuestos. Sin embargo, al no declarar estándares abiertos, la garantía de repuestos a 10 años depende de las marcas elegidas en cada proyecto. | **Where do I buy a spare part in 5 years?** → A través de las marcas utilizadas en cada proyecto. No hay un estándar abierto que garantice disponibilidad global independiente del integrador. |
| **D8 — Privacidad y soberanía de datos** | **2/5** | No hay política de privacidad visible ni declaración sobre dónde se alojan los datos. Los sistemas profesionales permiten operación local, pero el proveedor no lo comunica explícitamente. | **Does my data leave the country?** → No declara. Es una incógnita completa y el punto más débil de su perfil público. |

**Scoring criteria:** DSEM Section 2

## 4. Context Weighting (Argentina / Latin America)

| Dimensión | Weight | Score | Weighted |
| :--- | :--- | :--- | :--- |
| **D2 (Dependency)** | 25% | 3 | 0.75 |
| **D8 (Privacy)** | 20% | 2 | 0.40 |
| **D1 (Infrastructure)** | 15% | 3 | 0.45 |
| **D7 (Sustainability)** | 15% | 3 | 0.45 |
| **D3 (Functionality)** | 10% | 4 | 0.40 |
| **D6 (Transparency)** | 8% | 3 | 0.24 |
| **D5 (Complexity)** | 5% | 4 | 0.20 |
| **D4 (Value model)** | 2% | 4 | 0.08 |
| **TOTAL** | **100%** | | **3.09 / 5** |

## 5. Structural Profile (Escala /5)

| Profile | D1 | D2 | D7 | D8 | Score Range (/5) | Result |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 🔴 Red — Ultra light | 1-2 | 1-2 | 1-2 | 1 | 1.00 - 1.75 | ❌ |
| 🟠 Orange — Heavy closed | 4-5 | 2-3 | 2-3 | 2-3 | 2.25 - 3.25 | ❌ |
| 🟢 Green — Open hybrid | 3-4 | 3-4 | 3-4 | 4 | 3.00 - 3.75 | ✅ |
| 🔵 Blue — Balanced architecture | 4 | 4-5 | 4-5 | 4-5 | 3.75 - 4.50 | ❌ |
| ⚫ Black — Critical infrastructure | 5 | 5 | 5 | 5 | 4.50 - 5.00 | ❌ |

**Determined profile:** 🟢 **Green — Open hybrid**
**Descriptor:** "Instalación con ingeniería profesional, metodología de documentación avanzada, pero opacidad en privacidad de datos y estándares abiertos no declarados."

## 6. Summary of Structural Risks

| Risk Dimension | Observation |
| :--- | :--- |
| **Internet dependency** | **Bajo-medio.** No se indica uso de nube obligatoria general, pero dependerá de productos específicos en cada proyecto. La filosofía de documentación no aborda este punto. |
| **Vendor lock-in** | **Medio-bajo.** La filosofía de "documentación para el cliente" reduce teóricamente el lock-in. En la práctica, la dependencia del conocimiento del integrador original es moderada hasta que se valide la calidad documental. |
| **Spare parts / repairability** | **Medio.** Uso de marcas reconocidas facilita repuestos, pero al no declarar estándares abiertos, la disponibilidad a largo plazo depende de decisiones de producto de cada proyecto. |
| **Data sovereignty** | **Medio-bajo.** No hay política de datos pública clara. Es el punto ciego de su propuesta. |
| **Documentation / transparency** | **Medio.** Son excepcionalmente transparentes en su *filosofía* de documentación, pero opacos en tecnologías específicas (protocolos) y arquitecturas concretas. |

## 7. Conclusion

Trendhouse representa un **proveedor técnico maduro en el mercado argentino de domótica y soluciones integrales**. Su modelo se basa en **diseño profesional, integración de múltiples tecnologías y ejecución a medida**.

Es un caso atípico y valioso: **venden metodología tanto como tecnología**. Su filosofía de documentación entrega al cliente una herramienta que la mayoría de integradores retiene. Esto los posiciona como una opción estructuralmente sólida para un cliente cuyo mayor temor es quedar atado a un integrador que desaparezca.

**Fortalezas estructurales:**
*   ✅ **Profundidad funcional (D3):** Integración compleja de múltiples sistemas.
*   ✅ **Modelo de valor (D4):** Venden ingeniería, no dispositivos.
*   ✅ **Filosofía de documentación (D2/D7):** Enfoque pionero en independencia del integrador.

**Debilidades estructurales:**
*   ❌ **Opacidad en privacidad (D8):** No hay política de datos visible. Los sistemas profesionales permiten operación local, pero no se comunica.
*   ❌ **Estándares no declarados (D1):** No especifican protocolos abiertos, lo que dificulta evaluar interoperabilidad futura.

**Perfil DSEM: 🟢 Green — Open hybrid (3.09/5)**

Para un cliente que valore **independencia a largo plazo** por sobre especificaciones técnicas detalladas, Trendhouse es una opción de riesgo estructural moderado-bajo. Para un cliente técnico que quiera saber exactamente qué estándares y protocolos se usarán, necesitará profundizar en entrevistas personales.

## 8. Metadata

**License:** CC BY-SA 4.0
**Attribution:** DSEM v1.0 — Matias Cacciagrano, 2025
**Case study license:** Same as DSEM (open, share-alike)

*This case is a public contribution to the DSEM open standard.*
