
---

## 1. La Identidad como el Nuevo Perímetro

En la nube, la seguridad ya no está protegida por un perímetro físico (como las paredes de un centro de datos). En su lugar, el perímetro se define y gestiona a través de **identidades digitales**. Controlar estas identidades es la forma principal de dar acceso a los datos y evitar el uso no autorizado.

---

## 2. Las Tres "A" de la Gestión de Identidades

Para poner en práctica la seguridad, Google Cloud se basa en tres pilares fundamentales conocidos como las **Tres A**:

| Pila (La "A") | ¿Qué pregunta responde? | Definición y Herramientas |
| :--- | :--- | :--- |
| **Authentication**<br>(Autenticación) | **¿Quién eres?** | Es el guardián de acceso. Verifica que el usuario o sistema sea quien dice ser mediante credenciales (contraseñas, tokens físicos o datos biométricos). |
| **Authorization**<br>(Autorización) | **¿Qué tienes permitido hacer?** | Una vez identificado el usuario, determina a qué recursos tiene acceso y qué acciones puede ejecutar, basándose en sus roles y responsabilidades. |
| **Auditing / Accounting**<br>(Auditoría) | **¿Qué hiciste?** | Monitorea y rastrea las actividades de los usuarios dentro del sistema mediante la recolección de registros de actividad (*logs*). |

> [!TIP] Clave de Examen: Verificación en Dos Pasos (2SV / 2FA / MFA)
> Es una función de seguridad que añade una capa extra de protección a la **Autenticación**. Obliga al usuario a proporcionar dos tipos de información diferentes para iniciar sesión (ej. su contraseña habitual + un código enviado a su teléfono o generado en *Google Authenticator*). Esto hace que el acceso no autorizado sea extremadamente difícil, incluso si alguien te roba la contraseña.

> [!NOTE] Analogía de la Auditoría
> Funciona exactamente igual que las **cámaras de vigilancia de un centro comercial**. No detienen el acceso, pero mantienen un ojo vigilante registrando todo lo que pasa, lo cual es invaluable para investigar incidentes de seguridad, rastrear el cumplimiento legal (*compliance*) y evaluar el rendimiento del sistema.

---

## 3. IAM: Identity and Access Management

**IAM** es el centro de comando centralizado de Google Cloud para controlar **quién** puede hacer **qué** dentro de los recursos de tu organización. 

En lugar de configurar la seguridad servicio por servicio, IAM te da un panel único para:
*   Crear y gestionar cuentas de usuario.
*   Asignar **roles** y otorgar o revocar **permisos** específicos a los recursos.
*   Auditar la actividad de los usuarios.
*   Monitorear la postura de seguridad de la empresa de manera eficiente.

Gracias a IAM, las empresas obtienen un **control de acceso granular** (fino y detallado), máxima visibilidad y una gestión centralizada que protege los datos sensibles sin entorpecer el trabajo diario.

---

##  Enfoque de Negocio (Toma de Decisiones para el Examen)

*   **¿Qué herramienta de Google Cloud debes usar para definir qué empleados pueden ver una base de datos y cuáles pueden borrarla?** ➡️ **IAM (Identity and Access Management)**.
*   **¿A qué concepto corresponde la acción de obligar a los empleados a usar una contraseña y un token digital para entrar al sistema?** ➡️ **Autenticación (Authentication / 2SV)**.
*   **Si un auditor externo pide un registro histórico de quién modificó las configuraciones de los servidores el mes pasado, ¿qué pilar de seguridad se encarga de esto?** ➡️ **Auditoría (Auditing / Logs)**.
*   **¿Cuál es el beneficio de negocio de implementar IAM en la empresa?** ➡️ Proporcionar un **control de acceso granular y centralizado** para mitigar riesgos de filtración de datos de forma eficiente.