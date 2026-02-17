# Matriz de Comparación de Casos de Estudio — DSEM v1.0

Esta tabla resume los hallazgos estructurales clave de los casos de estudio publicados hasta la fecha. Permite una comparación rápida de perfiles de riesgo, fortalezas y debilidades de cada proveedor analizado.

| Caso | Perfil (DSEM) | Puntaje (/5) | Fortaleza Estructural Principal | Debilidad Crítica | Resumen para el Cliente |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **case-01.md** | 🔴 Red — Ultra light | 1.10 | **Ninguna.** Modelo de gadgets WiFi. | Dependencia total de nube. Sistema muere sin internet o si el proveedor desaparece. | **Riesgo máximo.** No es una instalación, es una compra de gadgets descartables. El cliente no es dueño de su sistema. |
| **case-02.md** | 🔴 Red — Ultra light | 1.52 | **Operación offline local.** Mitiga riesgo de caída de internet para control básico. | Protocolo inalámbrico propietario. Ecosistema 100% cautivo. Sin repuestos garantizados. | **Riesgo máximo.** Similar al caso-01, pero con la ventaja parcial de funcionar sin internet. Sigue siendo un ecosistema cerrado y descartable. |
| **case-03.md** | 🔴 Red — Ultra light | 1.17 | **Ninguna.** Marketing puro, cero transparencia técnica. | **Sin operación offline inteligente.** Sin internet, la domótica no funciona (solo operación manual). Opacidad total. | **Riesgo máximo.** Es el perfil más frágil de la muestra. El cliente compra una promesa, no una solución técnica. |
| **case-04.md** | 🔵 Blue — Balanced architecture | 3.27 | **Infraestructura profesional.** Basada en marcas premium (Crestron, Lutron, Control4). Sustentable y mantenible. | **Opacidad en privacidad de datos.** No informa sobre uso de nube ni destino de los datos del cliente. | **Riesgo moderado.** El cliente obtiene un sistema sólido y con futuro, pero desconoce completamente qué pasa con sus datos. |
| **case-05.md** | 🔵 Blue — Balanced architecture | 4.07 | **Estándar abierto (KNX).** Mantenibilidad garantizada por terceros. Infraestructura cableada, robusta y sustentable. | **Opacidad en privacidad de datos.** No explicita si la implementación es 100% local o usa nube, aunque KNX lo permite. | **Riesgo bajo.** Es el perfil más robusto. La única falta es no comunicar la soberanía de datos que técnicamente puede ofrecer. |

## Observaciones Generales

*   **El patrón de opacidad en datos (D8) es transversal:** Todos los casos, incluso los más robustos (case-04, case-05, case-06), fallan en comunicar públicamente el destino de los datos del cliente. Es el punto ciego de la industria en la muestra analizada.
*   **KNX y documentación marcan la diferencia:** Los casos con estándares abiertos (case-05) o metodologías de documentación (case-06) son los únicos que ofrecen una estrategia clara para la mantenibilidad futura.
*   **El perfil 🔴 Red es un "no comprar" estructural:** Los tres primeros casos representan un riesgo máximo para el cliente, ya que crean una dependencia absoluta de un proveedor con una barrera de salida altísima o directamente nula.
