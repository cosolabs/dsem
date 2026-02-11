# Análisis de Proveedor — DSEM v1.0

**Evaluación estructural según Domotics Structural Evaluation Model**  
**Metodología:** [github.com/cosolabs/dsem](https://github.com/cosolabs/dsem)  
**Fecha:** Febrero 2026 | **Fuente:** Sitio web del proveedor (publicado 2020)  
**Caso anonimizado para análisis público**

---

## Evaluación por dimensión

| Dimensión | Puntaje | Evidencia observable | Criterio DSEM |
|:---------|:------:|:---------------------|:--------------|
| **D1 — Infraestructura** | 1/5 | Solo WiFi. "Sin obras". No declara estándares abiertos (Zigbee, KNX, MQTT). | Nivel 1: Dispositivos solo WiFi / inalámbrico propietario, sin hub abierto. |
| **D2 — Dependencia operativa** | 1/5 | No menciona funcionamiento offline. No entrega documentación técnica. Sistema no rescatable si la empresa desaparece. | Nivel 1: Sistema muere sin su nube. |
| **D3 — Profundidad funcional** | 2/5 | Luces, cerraduras, aire, timbre, seguridad básica. Sin integración HVAC real, gestión energética ni lógica condicional avanzada. | Nivel 2: Luces + escenas. |
| **D4 — Modelo de valor** | 1/5 | Venta por dispositivo + instalación. No hay ingeniería a medida ni infraestructura. | Nivel 2: Venta de dispositivo + instalación. |
| **D5 — Complejidad estructural** | 1/5 | "Sin obras" = Plug & Play. No requiere plano, etapa de construcción ni tablero dedicado. | Nivel 1: Plug & Play. |
| **D6 — Transparencia tecnológica** | 1/5 | Solo marketing: familias felices, ambientes lindos, frases genéricas. No menciona protocolos, marcas ni arquitectura. | Nivel 1: Solo marketing de estilos de vida. |
| **D7 — Sustentabilidad del ecosistema** | 1/5 | No informa repuestos a futuro. Dependencia de marca no declarada. Perfil: hardware discontinuado en <2 años. | Nivel 1-2: Dependencia de una sola marca. Riesgo alto de discontinuación en <2 años. |
| **D8 — Privacidad y soberanía de datos** | 1/5 | No informa dónde se almacenan los datos. No ofrece opción local. Nube obligatoria, servidores no declarados. | Nivel 1: Nube obligatoria, servidores no declarados, telemetría oculta. |

---

## Ponderación para contexto Argentina/Latam

| Dimensión | Peso | Puntaje | Ponderado |
|:---------|:----:|:------:|:---------:|
| **D2 — Dependencia operativa** | 25% | 1 | 0.25 |
| **D8 — Privacidad y soberanía** | 20% | 1 | 0.20 |
| **D1 — Infraestructura** | 15% | 1 | 0.15 |
| **D7 — Sustentabilidad** | 15% | 1 | 0.15 |
| **D3 — Profundidad funcional** | 10% | 2 | 0.20 |
| **D6 — Transparencia tecnológica** | 8% | 1 | 0.08 |
| **D5 — Complejidad estructural** | 5% | 1 | 0.05 |
| **D4 — Modelo de valor** | 2% | 1 | 0.02 |
| **TOTAL** | **100%** | | **1.10 / 100** |

---

## Perfil estructural

# 🔴 ROJO — Ultra light

**"Gadgets, nube obligatoria, descartables."**

**Características del perfil:**
- D1: 1-2 | D2: 1-2 | D7: 1-2 | D8: 1
- Rango típico de puntaje: 20-35
- **Proveedor evaluado: 1.10**

---

## Conclusión

Este proveedor vende gadgets, no infraestructura domótica abierta y sustentable.

**✅ Puntos fuertes (si existen):**
- *Ninguno documentado.*

**❌ Riesgos estructurales críticos:**

| Riesgo | Evidencia | Consecuencia |
|--------|----------|--------------|
| **Dependencia de nube** | No menciona funcionamiento offline | Sistema inoperable sin internet. |
| **Protocolo cerrado** | Solo WiFi, sin estándares abiertos | Bloqueo total con la marca. Imposible expandir con terceros. |
| **Nube opaca** | No declara servidores ni jurisdicción | Datos personales y de ocupación sin soberanía. |
| **Obsolescencia programada** | Sin garantía de repuestos | Hardware con perfil de electrónica de consumo. |
| **Sin documentación técnica** | Solo manuales de usuario | El cliente no puede liberarse del integrador original. |

---

## Síntesis estructural

**El cliente no adquiere una instalación: adquiere una dependencia comercial y tecnológica.**

- No hay estándares abiertos.
- No hay funcionamiento sin internet.
- No hay documentación técnica para mantenimiento de terceros.
- No hay soberanía de datos (solo opción remota vía nube).
- No hay garantía de repuestos a mediano plazo.
- No hay transparencia: el sitio web muestra ambientes felices, no planos, protocolos ni arquitectura.

**El riesgo estructural es máximo. El perfil es Ultra light sin atenuantes.**

---

🔗 Análisis realizado según **DSEM v1.0** — Febrero 2026  
**Caso anonimizado para contribución al estándar abierto**  
[github.com/cosolabs/dsem](https://github.com/cosolabs/dsem)
