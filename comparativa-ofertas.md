# Plantilla Comparativa DSEM — Evaluación de Ofertas de Domótica

## Domotics Structural Evaluation Model v1.0

**Autor:** Matias Cacciagrano — 2025  
**Licencia:** CC BY-SA 4.0  
**Repositorio:** [github.com/cosolabs/dsem](https://github.com/cosolabs/dsem)  
**Formato recomendado:** Google Sheets / Excel (esta es la versión estructural para copiar)

---

## CÓMO USAR ESTA PLANTILLA

1. **Cree una hoja de cálculo** con las siguientes columnas.
2. **Ingrese los datos** de cada oferta según la evidencia recolectada.
3. **El puntaje se calcula automáticamente** (ponderación Latinoamérica incluida).
4. **Compare perfiles y riesgo**, no solo precio.

---

## 1. TABLA DE PONDERACIÓN (fija para la región)

| Dimensión | Peso |
|----------|------|
| D2 — Dependencia operativa | 25% |
| D8 — Privacidad y soberanía | 20% |
| D1 — Infraestructura | 15% |
| D7 — Sostenibilidad | 15% |
| D3 — Funcionalidad | 10% |
| D6 — Transparencia | 8% |
| D5 — Complejidad | 5% |
| D4 — Modelo de valor | 2% |
| **TOTAL** | **100%** |

---

## 2. PLANILLA DE EVALUACIÓN (estructura de columnas)

| Criterio | Peso | Oferta A | Oferta B | Oferta C | Oferta D |
|----------|------|----------|----------|----------|----------|
| **D1 — Infraestructura** (1-5) | 15% | | | | |
| *Evidencia requerida:* Protocolos declarados, tipo de hub, estándares | | | | | |
| **D2 — Dependencia** (1-5) | 25% | | | | |
| *Evidencia:* ¿Otro técnico puede mantenerlo? ¿Entregan credenciales? | | | | | |
| **D3 — Funcionalidad** (1-5) | 10% | | | | |
| *Evidencia:* Alcance real de integración | | | | | |
| **D4 — Modelo de valor** (1-5) | 2% | | | | |
| *Evidencia:* ¿Venden dispositivos, proyectos o infraestructura? | | | | | |
| **D5 — Complejidad** (1-5) | 5% | | | | |
| *Evidencia:* Etapa de obra requerida | | | | | |
| **D6 — Transparencia** (1-5) | 8% | | | | |
| *Evidencia:* ¿Publican esquemas y tecnologías? | | | | | |
| **D7 — Sostenibilidad** (1-5) | 15% | | | | |
| *Evidencia:* Repuestos en 5 años, hardware reprogramable | | | | | |
| **D8 — Privacidad** (1-5) | 20% | | | | |
| *Evidencia:* ¿Datos locales o nube? ¿Telemetría? | | | | | |
| | | | | | |
| **PUNTAJE PONDERADO** ( /100 ) | **100%** | **0.0** | **0.0** | **0.0** | **0.0** |
| **Perfil DSEM estimado** | | | | | |
| **Precio de oferta (USD/ARS)** | | | | | |
| **Relación puntaje/precio** | | | | | |

---

## 3. ESCALA DE VALORACIÓN POR DIMENSIÓN

| Nivel | D1 Infraestructura | D2 Dependencia | D7 Sostenibilidad | D8 Privacidad |
|-------|--------------------|----------------|-------------------|---------------|
| **1** | Solo WiFi/BT, sin hub | Muere sin su nube | Modelos <2 años | Nube extranjera, telemetría |
| **2** | Nube propia obligatoria | Offline pero no reprogramable | Marca única | Nube regional obligatoria |
| **3** | Hub físico, sin estándar | Solo ellos lo mantienen | Estándar + hardware cautivo | Híbrido (nube optativa) |
| **4** | Estándares abiertos | Otro integrador puede | Hardware reprogramable | Local por defecto |
| **5** | Bus cableado documentado | Cliente tiene todo | Comunidad + múltiples marcas | Local + open source |

---

## 4. EJEMPLO COMPARATIVO (caso simulado)

| Criterio | Peso | Oferta A (Marca X) | Oferta B (Gadgets) | Oferta C (KNX) | Oferta D (Abierto) |
|----------|------|---------------------|---------------------|----------------|---------------------|
| D1 | 15% | 4 | 2 | 5 | 4 |
| D2 | 25% | 
