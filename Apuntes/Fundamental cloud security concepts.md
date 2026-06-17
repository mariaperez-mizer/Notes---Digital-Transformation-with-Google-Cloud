
---
[[Cloud security components]]
[[Identity]]
[[Google´s secure-by-desing cloud platform]]
[[Quiz Fundamental cloud security concepts]]


## 1. Gobernanza de Acceso (Controlar quién entra)

Para reducir el riesgo de accesos no autorizados a datos sensibles por parte de los empleados, el examen evalúa tres modelos de control de identidad fundamentales:

*   **Modelo de Acceso Privilegiado (Privileged Access):** Otorga a usuarios específicos (como administradores de sistemas) un conjunto de permisos mucho más amplio que al usuario común para realizar tareas críticas (como restauración de datos o soporte técnico). *Nota del examen:* Debido a su alto poder, este acceso debe ser estrictamente monitoreado y gestionado.
*   **Principio de Menor Privilegio (Least Privilege):** Consiste en dar a los usuarios **únicamente los permisos mínimos necesarios** para realizar su trabajo diario. Por ejemplo, un vendedor solo debe tener acceso al CRM, pero no al sistema de nóminas o finanzas. Esto reduce masivamente el impacto si una cuenta llega a verse comprometida.
*   **Arquitectura de Cero Confianza (Zero-Trust Architecture):** Este modelo asume que **ningún** usuario o dispositivo es seguro por defecto, esté dentro o fuera de la red de la empresa. Todo usuario y dispositivo debe ser **autenticado y verificado continuamente** antes de poder acceder a cualquier recurso.

---

## 2. Defensa y Resiliencia en la Nube (Estrategia de Seguridad)

La seguridad no es un parche que se pone al final, sino una estrategia continua definida por tres conceptos clave:

> [!NOTE] Seguridad por Defecto (Security by Default)
> Es el principio de integrar las medidas de seguridad dentro de los sistemas y aplicaciones **desde las primeras etapas de su desarrollo**. Al diseñar pensando en la seguridad desde el día uno, se construye una base sólida en la nube.

*   **Postura de Seguridad (Security Posture):** Es el estado de seguridad general de todo tu entorno en la nube. Indica qué tan bien preparada está tu organización para defenderse de un ataque cibernético. Se evalúa comparando tus políticas y controles actuales contra **líneas base (baselines)** o marcos de seguridad internacionales.
*   **Ciberresiliencia (Cyber Resilience):** Es la capacidad de una organización no solo para defenderse, sino para **soportar un ataque y recuperarse rápidamente** de las interrupciones operativas, minimizando el impacto en el negocio.

---

## 3. Medidas de Protección de Recursos (Herramientas Técnicas)

Para proteger la infraestructura de amenazas externas o fugas de información, se utilizan tres herramientas esenciales:

| Concepto | Analogía / Definición | Propósito en la Nube |
| :--- | :--- | :--- |
| **Firewall (Cortafuegos)** | El **guardia de seguridad** de la red. | Revisa todo el tráfico entrante y saliente y, basándose en reglas predefinidas, decide qué tráfico es seguro dejar pasar y cuál bloquear para proteger servidores y bases de datos. |
| **Cifrado / Descifrado (Encryption / Decryption)** | Un **idioma secreto**. | El cifrado convierte los datos en un formato ilegible mediante un algoritmo. El descifrado vuelve a hacerlos legibles usando una **llave de cifrado (key)**. Si un atacante intercepta los datos, no podrá leerlos sin la llave. |
| **DLP (Data Loss Prevention)** | El **detector de fugas**. | Conjunto de herramientas y estrategias que identifican, monitorean y protegen automáticamente la información sensible (como números de tarjetas de crédito o identificaciones personales) para evitar que se pierda, se use mal o sea expuesta a usuarios no autorizados. |

> [!WARNING] Clave para el examen
> Proteger la **llave de cifrado** es tan importante como proteger los datos mismos, ya que quien posea la llave tiene el poder de descifrar y leer toda la información oculta.

---

## Enfoque de Negocio (Toma de Decisiones para el Examen)

*   **¿Cuál es la mejor práctica al asignar permisos a un nuevo empleado?** ➡️ Aplicar el **Principio de Menor Privilegio (Least Privilege)**.
*   **¿Qué modelo de seguridad elimina el concepto de "red interna confiable" y obliga a verificar siempre a todos?** ➡️ **Zero-Trust Architecture**.
*   **¿Qué solución debe implementar una empresa para evitar que se filtren por error números de tarjetas de crédito de sus clientes?** ➡️ **DLP (Data Loss Prevention)**.
*   **¿Cómo se le llama a la métrica que evalúa qué tan lista está una empresa contra ataques comparándose con un marco de referencia estándar?** ➡️ **Security Posture**.