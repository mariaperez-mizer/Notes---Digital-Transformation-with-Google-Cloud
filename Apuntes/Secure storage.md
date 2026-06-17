
---

## 1. El Cifrado como Estrategia de Defensa en Profundidad

Mientras que los muros y la biometría protegen los centros de datos físicos, el **cifrado (encryption)** protege los datos en sí mismos. Funciona como un código secreto: toma la información legible y utiliza algoritmos especiales para codificarla hasta convertirla en un formato completamente ilegible (*gibberish*).

> [!NOTE] La analogía de la caja fuerte indestructible
> Si un atacante lograra evadir a los guardias y robar físicamente un disco duro, los datos dentro de él serían incomprensibles. Es como meter tu información en una caja fuerte indestructible: aunque un ladrón se robe la caja completa, no podrá ver, entender ni manipular el contenido a menos que posea la **combinación exacta (la llave de cifrado)**.

---

## 2. Protección del Dato en sus Diferentes Estados

A diferencia de un objeto físico, los datos digitales se mueven e interactúan constantemente. Google Cloud protege la información aplicando cifrado de manera automática en todos sus estados:

### A) Datos en Reposo (Data at Rest)
Es la información que está almacenada estáticamente en dispositivos físicos (discos duros, servidores, almacenamiento en la nube).
*   **En Google Cloud:** Todo el contenido de los clientes se cifra **automáticamente por defecto y de forma gratuita**, sin necesidad de configuraciones adicionales.
*   **Cloud KMS (Key Management Service):** Si una empresa prefiere tener el control total y gestionar sus propias llaves de cifrado (en lugar de dejar que Google las administre), puede utilizar este servicio.

### B) Datos en Tránsito (Data in Transit)
Es la información que se está moviendo a través de redes o internet (por ejemplo, cuando un usuario envía datos a una aplicación web).
*   **En Google Cloud:** Se encripta y autentica la información en múltiples capas de red, protegiéndola contra intercepciones de ciberdelincuentes, especialmente cuando viaja fuera de las fronteras físicas controladas por Google.

### C) Datos en Uso / En Memoria (Data in Use / in Memory)
Es la información que la computadora o servidor está **procesando activamente** en su memoria RAM en un momento determinado.
*   **En Google Cloud:** Tradicionalmente, los datos debían descifrarse en memoria para ser procesados. Google implementa tecnologías de cifrado de memoria para bloquear los datos dentro de la memoria del sistema, evitando accesos físicos no autorizados al hardware de cómputo.

---

## 3. Computación Confidencial (Confidential Computing)

Este es uno de los mayores diferenciadores tecnológicos de Google Cloud y un concepto clave para el examen. 

> [!TIP] Examen: Confidential Computing
> Es una plataforma avanzada que **mantiene los datos cifrados en la memoria RAM mientras están siendo procesados**. Utiliza hardware especializado para crear un espacio privado y totalmente aislado en el procesador.
> *   **Beneficio supremo de negocio:** Garantiza que absolutamente nadie, **ni siquiera los empleados de Google con acceso físico al servidor**, pueda ver o acceder a la información sensible mientras la aplicación la procesa.
> *   **Servicios compatibles:** Está disponible para *Confidential VMs*, *Google Kubernetes Engine (GKE)*, *Dataflow*, *Apache Spark* y *Confidential Space*.

---

## 4. Estándares Globales de Cifrado Utilizados

Google no inventa sus propios algoritmos de cifrado; utiliza los estándares de seguridad más respetados y confiables del mundo:

*   **AES-256 (Advanced Encryption Standard):** Es el estándar global utilizado por gobiernos y líderes tecnológicos. Google lo usa **por defecto** para proteger los **datos en reposo**.
*   **TLS (Transport Layer Security):** Protocolo criptográfico de vanguardia empleado por Google para cifrar y validar estrictamente los **datos en tránsito** a medida que se mueven por la red.

---

##  Enfoque de Negocio (Toma de Decisiones para el Examen)

*   **¿Cuánto cuesta o qué configuración requiere el cifrado de datos en reposo en Google Cloud?** ➡️ Es **gratuito, automático y viene activado por defecto** para todos los clientes.
*   **¿Qué servicio debe elegir una empresa si su departamento legal le exige administrar sus propias llaves de cifrado en la nube?** ➡️ **Cloud KMS (Key Management Service)**.
*   **¿Qué tecnología de Google Cloud elegirías para procesar datos bancarios o médicos ultra confidenciales, asegurando que ni el proveedor de la nube pueda verlos?** ➡️ **Confidential Computing (ej. Confidential VMs)**.
*   **¿Qué estándar de la industria utiliza Google Cloud para proteger los datos almacenados en sus discos?** ➡️ **AES-256**.
*   **¿Qué protocolo asegura los datos del cliente mientras viajan por las redes de Google?** ➡️ **TLS**.