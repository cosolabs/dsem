# Análisis de Proveedor — DSEM v1.0

**Evaluación estructural según Domotics Structural Evaluation Model**  
**Metodología:** [github.com/cosolabs/dsem](https://github.com/cosolabs/dsem)  
**Fecha:** Febrero 2026 | **Fuente:** Sitio web del proveedor (material promocional)  
**Caso anonimizado para análisis público**

---

## Evaluación por dimensión

| Dimensión | Puntaje | Evidencia observable | Criterio DSEM |
|:---------|:------:|:---------------------|:--------------|
| **D1 — Infraestructura** | 1/5 | Protocolo inalámbrico propietario ("WiBus"). No declara estándares abiertos (Zigbee, KNX, MQTT, DALI). No menciona hub físico ni arquitectura cableada. | Nivel 1: Dispositivos solo WiFi / inalámbrico propietario, sin hub abierto. |
| **D2 — Dependencia operativa** | 2/5 | Funciona offline en red local. No menciona documentación técnica para que otro integrador lo mantenga. Sistema autónomo pero cautivo de su software/app. | Nivel 2: Funciona offline pero no puede ser reprogramado por terceros. Solo el proveedor puede mantenerlo. |
| **D3 — Profundidad funcional** | 3/5 | Controla iluminación, climatización, seguridad, cortinados, audio multiroom. No menciona lógica condicional avanzada (ej. reglas "si-entonces" cruzadas) ni gestión energética con histórico. | Nivel 3: Luces + HVAC + seguridad. Sin coordinación compleja multi-sistema documentada. |
| **D4 — Modelo de valor** | 2/5 | "Soluciones accesibles adaptadas a tu presupuesto". Costo "varía según el proyecto". No se evidencia ingeniería a medida; esquema de dispositivo + instalación. | Nivel 2: Venta de dispositivo + instalación. |
| **D5 — Complejidad estructural** | 2/5 | Instalación en viviendas existentes "sin necesidad de cableado adicional". No requiere planificación arquitectónica ni tablero dedicado. | Nivel 2: Instalación eléctrica básica. "Sin obras". |
| **D6 — Transparencia tecnológica** | 1/5 | Marketing puro: "experiencia innovadora", "ambientes personalizados", "entorno inteligente". No menciona protocolos, frecuencias, marcas de hardware, topología ni arquitectura de red. | Nivel 1: Solo marketing de estilos de vida. |
| **D7 — Sustentabilidad del ecosistema** | 1/5 | No informa sobre repuestos a futuro. Protocolo propietario genera dependencia total de marca. Hardware discontinuable sin soporte garantizado. | Nivel 1-2: Dependencia de una sola marca. Riesgo alto de discontinuación en <2 años. |
| **D8 — Privacidad y soberanía de datos** | 1/5 | No informa dónde se almacenan los datos. Control remoto requiere nube obligatoria. No ofrece opción local pura sin paso por servidores externos. | Nivel 1: Nube obligatoria, servidores no declarados, telemetría oculta. |

---

## Ponderación para contexto Argentina/Latam

| Dimensión | Peso | Puntaje | Ponderado |
|:---------|:----:|:------:|:---------:|
| **D2 — Dependencia operativa** | 25% | 2 | 0.50 |
| **D8 — Privacidad y soberanía** | 20% | 1 | 0.20 |
| **D1 — Infraestructura** | 15% | 1 | 0.15 |
| **D7 — Sustentabilidad** | 15% | 1 | 0.15 |
| **D3 — Profundidad funcional** | 10% | 3 | 0.30 |
| **D6 — Transparencia tecnológica** | 8% | 1 | 0.08 |
| **D5 — Complejidad estructural** | 5% | 2 | 0.10 |
| **D4 — Modelo de valor** | 2% | 2 | 0.04 |
| **TOTAL** | **100%** | | **1.52 / 100** |

---

## Perfil estructural

# 🔴 ROJO — Ultra light

**"Gadgets inalámbricos propietarios, ecosistema cautivo, descartables."**

**Características del perfil:**
- D1: 1-2 | D2: 1-2 | D7: 1-2 | D8: 1
- Rango típico de puntaje: 20-35
- **Proveedor evaluado: 1.52**

---

## Conclusión

Este proveedor vende un ecosistema cerrado de gadgets, no infraestructura domótica abierta y sustentable.

**✅ Puntos fuertes:**
- El sistema funciona sin internet en red local (D2+), mitigando parcialmente el riesgo de dependencia de nube para operación cotidiana.
- Sin costo de mantenimiento mensual declarado.

**❌ Riesgos estructurales críticos:**

| Riesgo | Evidencia | Consecuencia |
|--------|----------|--------------|
| **Protocolo propietario** | "WiBus" no es estándar abierto | Bloqueo total con la marca. Si el proveedor desaparece, el sistema no puede expandirse ni repararse con terceros. |
| **Nube opaca** | No declara servidores ni jurisdicción | Los datos de ocupación, hábitos y accesos salen del país sin consentimiento explícito ni opción local. |
| **Obsolescencia programada implícita** | Sin garantía de repuestos a 5 años | Hardware con perfil de electrónica de consumo, no de instalación eléctrica. |
| **Inexistencia de documentación técnica** | Solo manuales de usuario | El cliente no puede liberarse del integrador original. |

---

## Síntesis estructural

**El cliente no adquiere una instalación: adquiere una dependencia comercial y tecnológica.**

- No hay estándares abiertos.
- No hay soberanía de datos (solo opción remota vía nube).
- No hay documentación técnica para mantenimiento de terceros.
- No hay garantía de repuestos a mediano plazo.
- No hay transparencia: el sitio web muestra ambientes felices, no planos, protocolos ni arquitectura.

**El riesgo estructural es máximo. El perfil es Ultra light con agravante de cautividad posventa.**

---

🔗 Análisis realizado según **DSEM v1.0** — Febrero 2026  
**Caso anonimizado para contribución al estándar abierto**  
[github.com/cosolabs/dsem](https://github.com/cosolabs/dsem)
