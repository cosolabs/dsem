# Análisis de Proveedor — DSEM v1.0

## 1. Case Metadata

| Field | Value |
|-------|-------|
| **Case ID** | `case-02.md` |
| **Title** | Proveedor de domótica inalámbrica con protocolo propietario y operación offline |
| **Evaluator** | Anónimo |
| **Date** | 2026-02-11 |
| **Evidence source(s)** | Sitio web del proveedor (material promocional) |
| **Anonymization note** | Se han eliminado todas las marcas, nombres e identificadores del proveedor, incluyendo el nombre de su protocolo propietario. |

---

## 2. Provider / Proposal Summary

| Aspect | Description |
|--------|-------------|
| **Value proposition** | "Solución integrada que permite automatizar todo tipo de ambientes y espacios de manera inteligente. Control total desde app móvil. Funciona sin internet." |
| **Business model** | Venta de dispositivos + instalación. Sin costo de mantenimiento mensual. |
| **Target client** | Residencial (obra existente), hoteles, oficinas, retail, centros médicos, embarcaciones. |
| **Declared technology** | Protocolo inalámbrico **propietario**. No declara estándares abiertos (Zigbee, KNX, MQTT, DALI). No menciona hub físico ni arquitectura cableada. |

---

## 3. DSEM Dimensional Scoring

| Dimensión | Score (1-5) | Evidencia observable | Detector Question Answered |
|----------|-------------|---------------------|---------------------------|
| **D1 — Infraestructura** | 1/5 | Protocolo inalámbrico **propietario**. No declara estándares abiertos. No menciona hub físico ni arquitectura cableada. | *What protocols? What other brands can I connect?* → **Protocolo cerrado. No admite otras marcas.** |
| **D2 — Dependencia operativa** | 2/5 | **Funciona offline** en red local. No menciona documentación técnica para que otro integrador lo mantenga. Sistema autónomo pero cautivo de su software/app. | *If you don't exist tomorrow, who fixes it?* → **Solo ellos. No hay documentación para terceros.** |
| **D3 — Profundidad funcional** | 3/5 | Controla iluminación, climatización, seguridad, cortinados, audio multiroom. No menciona lógica condicional avanzada ni gestión energética con histórico. | *Example where two systems talk to each other?* → **No se evidencia lógica cruzada documentada.** |
| **D4 — Modelo de valor** | 2/5 | "Soluciones accesibles adaptadas a tu presupuesto". Costo "varía según el proyecto". Esquema de dispositivo + instalación. | *How do you quote: per device, per hour, per project?* → **Por dispositivo + instalación.** |
| **D5 — Complejidad estructural** | 2/5 | Instalación en viviendas existentes "sin necesidad de cableado adicional". No requiere planificación arquitectónica ni tablero dedicado. | *At what stage of construction do you get involved?* → **Solo retrofit, sin planificación.** |
| **D6 — Transparencia tecnológica** | 1/5 | **Marketing puro**: "experiencia innovadora", "ambientes personalizados", "entorno inteligente". No menciona protocolos, frecuencias, marcas de hardware, topología ni arquitectura. | *Website: technology or just pretty photos?* → **Solo fotos y frases aspiracionales.** |
| **D7 — Sustentabilidad del ecosistema** | 1/5 | No informa sobre repuestos a futuro. Protocolo propietario genera dependencia total de marca. Hardware discontinuable sin soporte garantizado. | *Where do I buy a spare part in 5 years?* → **No responde. Sin garantía de repuestos.** |
| **D8 — Privacidad y soberanía de datos** | 1/5 | No informa dónde se almacenan los datos. Control remoto **requiere nube obligatoria**. No ofrece opción local pura sin paso por servidores externos. | *Does my data leave the country?* → **No declara. Nube obligatoria para acceso remoto.** |

**Scoring criteria:** [DSEM Section 2](https://github.com/cosolabs/dsem?tab=readme-ov-file#2-the-8-structural-dimensions)

---

## 4. Context Weighting (Argentina / Latin America)

| Dimensión | Weight | Score | Weighted |
|----------|--------|-------|----------|
| D2 (Dependency) | 25% | 2 | 0.50 |
| D8 (Privacy) | 20% | 1 | 0.20 |
| D1 (Infrastructure) | 15% | 1 | 0.15 |
| D7 (Sustainability) | 15% | 1 | 0.15 |
| D3 (Functionality) | 10% | 3 | 0.30 |
| D6 (Transparency) | 8% | 1 | 0.08 |
| D5 (Complexity) | 5% | 2 | 0.10 |
| D4 (Value model) | 2% | 2 | 0.04 |
| **TOTAL** | **100%** | | **1.52 / 100** |

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
**Descriptor:** *"Gadgets inalámbricos propietarios, ecosistema cautivo, descartables."*

🔗 [DSEM Section 4 — Structural Profiles](https://github.com/cosolabs/dsem?tab=readme-ov-file#4-structural-profiles)

---

## 6. Summary of Structural Risks

| Risk Dimension | Observation |
|----------------|-------------|
| **Internet dependency** | **Mitigado parcialmente.** Funciona offline en red local. El control remoto sí requiere nube. |
| **Vendor lock-in** | **Crítico.** Protocolo propietario. Bloqueo total con la marca. Imposible integrar equipos de terceros. |
| **Spare parts / repairability** | **Crítico.** No informa repuestos a futuro. Hardware con perfil de electrónica de consumo, discontinuable sin soporte garantizado. |
| **Data sovereignty** | **Crítico.** Nube obligatoria para control remoto. No declara servidores ni jurisdicción. Datos de ocupación y hábitos sin soberanía. |
| **Documentation / transparency** | **Crítico.** Solo manuales de usuario. No hay documentación técnica para mantenimiento de terceros. |
| **Functional limitations** | **Moderado.** Controla iluminación, climatización, seguridad, cortinados, audio. Sin lógica condicional avanzada ni gestión energética con histórico. |

---

## 7. Conclusion

**Este proveedor vende un ecosistema cerrado de gadgets, no infraestructura domótica abierta y sustentable.**

El perfil **🔴 Ultra light** indica que el cliente no adquiere una instalación técnica, sino una **dependencia comercial y tecnológica**. A diferencia del caso-01, este sistema **funciona sin internet** en red local, lo que mitiga parcialmente el riesgo de dependencia de nube para operación cotidiana.

Sin embargo, los riesgos estructurales críticos persisten: **protocolo propietario, nube opaca para acceso remoto, nula garantía de repuestos, ausencia de documentación técnica y marketing sin transparencia tecnológica**.

**Riesgo estructural: MÁXIMO.**  
El perfil es Ultra light con **agravante de cautividad posventa**. Si el proveedor desaparece o discontinuúa la línea, el sistema no puede expandirse, repararse con terceros ni migrar a otro ecosistema.

---

## 8. Metadata

**License:** CC BY-SA 4.0  
**Attribution:** DSEM v1.0 — Matias Cacciagrano, 2025  
**Case study license:** Same as DSEM (open, share-alike)

*This case is an anonymized contribution to the DSEM open standard.*

🔗 [github.com/cosolabs/dsem](https://github.com/cosolabs/dsem)
