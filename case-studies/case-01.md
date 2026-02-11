# Análisis de Proveedor — DSEM v1.0

**Evaluación estructural según Domotics Structural Evaluation Model**  
Metodología: [github.com/cosolabs/dsem](https://github.com/cosolabs/dsem)  
Fecha: Febrero 2026 | Fuente: Sitio web del proveedor (publicado 2020)  
Caso anonimizado para análisis público

---

## Evaluación por dimensión

| Dimensión | Puntaje | Evidencia observable | Criterio |
|----------|--------|----------------------|----------|
| **D1 — Infraestructura** | 1/5 | Solo WiFi. "Sin obras". No declara estándares abiertos (Zigbee, KNX, MQTT). | [DSEM D1](https://github.com/cosolabs/dsem?tab=readme-ov-file#d1--infrastructure) |
| **D2 — Dependencia operativa** | 1/5 | No menciona funcionamiento offline. No entrega documentación técnica. Sistema no rescatable si la empresa desaparece. | [DSEM D2](https://github.com/cosolabs/dsem?tab=readme-ov-file#d2--operational-dependency) |
| **D3 — Profundidad funcional** | 2/5 | Luces, cerraduras, aire, timbre, seguridad básica. Sin integración HVAC real, gestión energética ni lógica condicional avanzada. | [DSEM D3](https://github.com/cosolabs/dsem?tab=readme-ov-file#d3--functional-depth) |
| **D4 — Modelo de valor** | 1/5 | Venta por dispositivo + instalación. No hay ingeniería a medida ni infraestructura. | [DSEM D4](https://github.com/cosolabs/dsem?tab=readme-ov-file#d4--value-model) |
| **D5 — Complejidad estructural** | 1/5 | "Sin obras" = Plug & Play. No requiere plano, etapa de construcción ni tablero dedicado. | [DSEM D5](https://github.com/cosolabs/dsem?tab=readme-ov-file#d5--structural-complexity) |
| **D6 — Transparencia tecnológica** | 1/5 | Solo marketing: familias felices, ambientes lindos, frases genéricas. **No menciona protocolos, marcas ni arquitectura.** | [DSEM D6](https://github.com/cosolabs/dsem?tab=readme-ov-file#d6--technological-transparency) |
| **D7 — Sustentabilidad del ecosistema** | 1/5 | No informa repuestos a futuro. Dependencia de marca no declarada. Perfil: hardware discontinuado en <2 años. | [DSEM D7](https://github.com/cosolabs/dsem?tab=readme-ov-file#d7--ecosystem-sustainability) |
| **D8 — Privacidad y soberanía de datos** | 1/5 | No informa dónde se almacenan los datos. No ofrece opción local. Nube obligatoria, servidores no declarados. | [DSEM D8](https://github.com/cosolabs/dsem?tab=readme-ov-file#d8--privacy-and-data-sovereignty) |

---

## Ponderación para contexto Argentina/Latam

| Dimensión | Peso | Puntaje | Ponderado |
|----------|------|---------|-----------|
| D2 (Dependencia) | 25% | 1 | 0.25 |
| D8 (Privacidad) | 20% | 1 | 0.20 |
| D1 (Infraestructura) | 15% | 1 | 0.15 |
| D7 (Sustentabilidad) | 15% | 1 | 0.15 |
| D3 (Funcionalidad) | 10% | 2 | 0.20 |
| D6 (Transparencia) | 8% | 1 | 0.08 |
| D5 (Complejidad) | 5% | 1 | 0.05 |
| D4 (Modelo valor) | 2% | 1 | 0.02 |
| **TOTAL** | **100%** | | **1.10 / 100** |

🔗 [Tabla de ponderación DSEM](https://github.com/cosolabs/dsem?tab=readme-ov-file#3-context-weighting)

---

## Perfil estructural

# 🔴 ROJO — Ultra light

> *"Gadgets, nube obligatoria, descartables."*

**Características del perfil:**  
- D1: 1-2 | D2: 1-2 | D7: 1-2 | D8: 1  
- Puntaje típico: 20-35  
- **Proveedor evaluado: 1.10**

🔗 [Tabla de perfiles DSEM](https://github.com/cosolabs/dsem?tab=readme-ov-file#4-structural-profiles)

---

## Conclusión

**Este proveedor vende gadgets, no infraestructura.**  
- No hay estándares abiertos.  
- No hay funcionamiento sin internet.  
- No hay documentación técnica.  
- No hay soberanía de datos.  
- No hay garantía de repuestos.  
- No hay transparencia.

**El riesgo estructural es máximo.**  
El cliente no compra una instalación: **compra una dependencia.**

---

*Análisis realizado según DSEM v1.0 — Febrero 2026*  
🔗 [github.com/cosolabs/dsem](https://github.com/cosolabs/dsem)  
*Caso anonimizado para contribución al estándar abierto*
