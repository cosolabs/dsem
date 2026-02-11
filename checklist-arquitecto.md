# Checklist del Arquitecto — DSEM v1.0

## Domotics Structural Evaluation Model

**Autor:** Matias Cacciagrano — 2025  
**Licencia:** CC BY-SA 4.0  
**Repositorio:** [github.com/cosolabs/dsem](https://github.com/cosolabs/dsem)  
**Uso:** Libre para copiar, pegar y adaptar en pliegos de licitación.

---

## CÓMO USAR ESTE DOCUMENTO

1. **Copie y pegue** el bloque de texto de la Sección 2 directamente en su pliego.
2. **Exija** a cada proveedor que complete la tabla de autoevaluación (Sección 3).
3. **Compare** las ofertas usando la plantilla comparativa (DSEM Matrix).
4. **Adjudique** no por precio, sino por perfil estructural y riesgo.

---

## 1. LAS 5 PREGUNTAS QUE TODO PLIEGO DEBERÍA HACER

Antes de escribir el pliego, pregunte al proveedor candidato:

| # | Pregunta | Lo que busca |
|---|---------|-------------|
| 1 | "¿El sistema funciona 100% sin internet?" | Independencia de nube |
| 2 | "¿Dónde compro un repuesto en 5 años?" | Sostenibilidad / Commodity |
| 3 | "¿Otro técnico puede mantenerlo?" | No vendor lock-in |
| 4 | "¿Me entregan las credenciales y planos?" | Soberanía del cliente |
| 5 | "¿Qué dispositivos de otras marcas puedo conectar?" | Estándar abierto real |

**Si responden "No" o "Depende" más de dos veces, descarte la oferta.**

---

## 2. TEXTO PARA PLIEGO DE LICITACIÓN (LISTO PARA COPIAR Y PEGAR)

---
### ANEXO TÉCNICO — SISTEMA DE DOMÓTICA

El sistema de domótica ofertado deberá cumplir con los siguientes requisitos estructurales mínimos:

**1. Independencia de infraestructura**
- El sistema deberá mantener todas sus funcionalidades básicas (encendido, apagado, escenas, automatizaciones horarias) ante una interrupción total del servicio de internet.
- No se admitirán sistemas que requieran nube obligatoria para operaciones locales.

**2. Estándares abiertos**
- El sistema deberá utilizar explícitamente estándares abiertos y documentados (Zigbee, KNX, Modbus, MQTT, DALI, LoRa o equivalentes).
- Se valorará positivamente la capacidad de integrar dispositivos de diferentes fabricantes bajo el mismo estándar.

**3. Sostenibilidad y repuestos**
- El hardware deberá tener disponibilidad de repuestos en el mercado local por un período mínimo de 5 años.
- Se penalizarán sistemas con hardware cautivo o de importación exclusiva.

**4. Documentación y transferencia**
- El instalador entregará al comitente:
  - Plano de ubicación de todos los dispositivos.
  - Topología de red.
  - Credenciales completas de administración.
  - Respaldo de la programación (si corresponde).
- El sistema deberá poder ser mantenido por otro integrador sin depender del instalador original.

**5. Protección eléctrica**
- Todos los dispositivos conectados a red eléctrica deberán estar respaldados por protecciones diferenciales y termomagnéticas en tablero.
- No se admitirán dispositivos enchufables sin protección aguas arriba.

**6. Suscripciones**
- El sistema no requerirá ningún tipo de suscripción, membresía o pago recurrente para su funcionamiento completo y permanente.
- Se declararán por escrito todos los servicios que eventualmente pudieran tener costo asociado.

---

## 3. FORMULARIO DE AUTOEVALUACIÓN PARA PROVEEDORES

*Entregar este formulario completo junto con la oferta.*

| Dimensión | Nivel (1-5) | Evidencia / Comentario |
|----------|-------------|------------------------|
| **D1 — Infraestructura**<br>¿Qué estándares usa? | | |
| **D2 — Dependencia**<br>¿Qué pasa si uds. no existen? | | |
| **D3 — Funcionalidad**<br>¿Qué integra realmente? | | |
| **D4 — Modelo de valor**<br>¿Cómo cotizan? | | |
| **D5 — Complejidad**<br>¿En qué etapa intervienen? | | |
| **D6 — Transparencia**<br>¿Publican esquemas? | | |
| **D7 — Sostenibilidad**<br>¿Repuestos en 5 años? | | |
| **D8 — Privacidad**<br>¿Dónde van los datos? | | |

**Declaro que la información aquí volcada es verídica y corresponde a la oferta presentada.**

Firma: ......................................................................  
Empresa: ......................................................................  
Fecha: ......................................................................  

---

## 4. SEMÁFORO DE ADJUDICACIÓN RÁPIDO

| Resultado | Perfil DSEM | Decisión |
|-----------|-------------|----------|
| **4-8 respuestas "Sí" en preguntas clave** | Verde / Azul | Adjudicar. Bajo riesgo. |
| **2-4 respuestas "Sí"** | Naranja | Analizar en profundidad. Pedir garantías. |
| **0-2 respuestas "Sí"** | Rojo | Rechazar. Riesgo estructural alto. |

---

## 5. REFERENCIAS

Este checklist es parte del **DSEM (Domotics Structural Evaluation Model)**, un estándar abierto para evaluar propuestas de domótica por evidencia observable, no por marketing.

- Repositorio oficial: [github.com/cosolabs/dsem](https://github.com/cosolabs/dsem)
- Licencia: CC BY-SA 4.0
- Autor: Matias Cacciagrano, 2025

---

**Versión 1.0 — Marzo 2025**
