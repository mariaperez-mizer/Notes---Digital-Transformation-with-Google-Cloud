

---

## 1. La Tríada CIA (El Fundamento de la Seguridad)

Para diseñar cualquier sistema de seguridad efectivo en la nube, el examen se basa en un modelo estándar de tres principios esenciales conocido como la **Tríada CIA** (*Confidentiality, Integrity, Availability*):

*   **Confidencialidad (Confidentiality):** Mantener la información importante a salvo y en secreto. Garantiza que **solo las personas autorizadas** puedan acceder a los datos sensibles, sin importar dónde estén guardados o hacia dónde se envíen.
    *   *Herramienta clave:* El **cifrado (encryption)** de datos y la protección estricta de las llaves de cifrado.
*   **Integridad (Integridad):** Mantener los datos **exactos, completos y confiables**. Asegura que la información no sea alterada, corrompida o manipulada de forma no autorizada durante su almacenamiento o transmisión (como asegurarse de que un mensaje no cambie en el camino).
    *   *Herramientas clave:* Controles de integridad como **checksums** (sumas de verificación) o **firmas digitales**.
*   **Disponibilidad (Availability):** Asegurar que los sistemas y servicios estén **siempre accesibles** y listos para ser usados por las personas autorizadas cuando lo necesiten (como tener luz eléctrica que nunca se corta).
    *   *Estrategias clave:* Diseñar arquitecturas con **redundancia**, mecanismos de **conmutación por error (failover)** y planes de **recuperación ante desastres**.

---

## 2. El Balance de la Tríada CIA

> [!WARNING] Concepto de Examen: El conflicto de prioridades
> Los tres principios de la tríada CIA pueden competir entre sí. Por ejemplo, si aumentas drásticamente la *confidencialidad* implementando un cifrado ultra complejo con múltiples capas de autenticación, podrías ralentizar el sistema o complicar el acceso, afectando negativamente la *disponibilidad*. El reto del negocio es **balancear estas prioridades** según sus necesidades operativas.

---

## 3. Operacionalizar la Seguridad: Control y Cumplimiento

Para llevar la teoría de la tríada CIA a la práctica dentro de una empresa, se necesitan dos componentes operativos críticos:

### A) Control
Se refiere a las **políticas y salvaguardas técnicas** tangibles que se implementan para mitigar los riesgos de seguridad.
*   *Ejemplos:* Autenticación robusta (como el uso de doble factor de forma obligatoria), restricciones de acceso basadas en roles y firewalls. Su objetivo es asegurar que solo los usuarios permitidos interactúen con la nube.

### B) Cumplimiento (Compliance)
Es la **adhesión estricta a las leyes, regulaciones y estándares de la industria** (como el resguardo de datos médicos o financieros de los clientes).
*   *Beneficio de negocio:* Cumplir con estas obligaciones legales demuestra el compromiso de la empresa con la privacidad, construye confianza con los clientes y accionistas, y minimiza riesgos de demandas o multas costosas.
*   *Ventaja de la nube:* Las organizaciones pueden **aprovechar las certificaciones oficiales de Google Cloud** (que ya cumple con auditorías internacionales) para cumplir con sus propios requisitos regulatorios de forma más fácil y económica.

---

## Enfoque de Negocio (Toma de Decisiones para el Examen)

*   **¿Qué principio de la tríada CIA se asegura de que un archivo de base de datos no sea modificado maliciosamente por un tercero?** ➡️ **Integridad (Integrity)**.
*   **¿Cuál es el beneficio de negocio de la "Disponibilidad" en la nube?** ➡️ Promover la **continuidad del negocio** ante cualquier interrupción o desastre técnico.
*   **¿Cómo puede una empresa acelerar su proceso de auditoría legal al mudarse a la nube?** ➡️ **Aprovechando las certificaciones de cumplimiento (compliance)** que Google Cloud ya posee en su infraestructura.
*   **¿A qué componente se refieren las restricciones de acceso y contraseñas seguras para mitigar riesgos?** ➡️ Al **Control**.