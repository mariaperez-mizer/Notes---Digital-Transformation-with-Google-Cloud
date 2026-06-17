
## 1. ¿Qué es Serverless Computing (Computación Servidor)?

El término **Serverless** (sin servidor) es un mito: **los servidores sí existen**, pero están completamente abstraídos. El desarrollador no tiene que aprovisionar, gestionar, actualizar ni parchar ninguna infraestructura; solo proporciona el código y Google Cloud se encarga de todo lo demás de forma automática en segundo plano.

> [!NOTE] Analogías clave para entender el modelo
> *   **El restaurante:** Pides la comida y aparece en tu mesa. Sabes que hay una cocina al fondo, pero no necesitas saber cómo funciona el horno.
> *   **El taxi:** Solo pagas cuando las ruedas se están moviendo y te están llevando a tu destino, no le pagas al conductor por estar estacionado en tu entrada "por si acaso".

###  Function as a Service (FaaS) y Modelos Basados en Eventos
En el mundo serverless, una **función** es una pieza de código diseñada para una tarea única y específica. 
Este modelo es **orientado a eventos (event-driven)**: el código permanece inactivo hasta que un "disparador" o *trigger* (ej. un usuario hace clic en "subir recibo", se sube un archivo o cambia algo en la base de datos) activa la función. Se ejecuta en una fracción de segundo y, en cuanto termina la tarea, se apaga por completo.

---

## 2. Productos (Serverless) de Google Cloud

Google Cloud ofrece tres herramientas serverless principales. Para el examen, debes saber exactamente cuándo elegir cada una:

### A) Cloud Run (Contenedores Serverless)
Es un entorno totalmente administrado para ejecutar **aplicaciones contenedorizadas**.
*   **Flexibilidad:** Soporta cualquier lenguaje o librería (siempre que se pueda meter en un contenedor).
*   **Escalado:** Escala automáticamente según el tráfico, e incluso **escala a cero** cuando no hay peticiones (costo \$0 por tiempo inactivo).
*   **Uso ideal:** Aplicaciones web modernas y servicios sin estado (*stateless*). **Es la opción preferida por Google actualmente.**

### B) Cloud Run Functions (Código Serverless / FaaS)
*(Anteriormente conocido como Cloud Functions)*. Es una plataforma para alojar **funciones simples y de propósito único**.
*   **Modelo:** 100% basado en eventos y automatizaciones ligeras.
*   **Uso ideal:** Enviar una notificación al móvil cuando se genera una orden, procesar una imagen justo cuando se sube a un almacenamiento, o conectar servicios mediante mensajes de Pub/Sub.

### C) App Engine (Plataforma como Servicio - PaaS)
Es un servicio integral (PaaS) diseñado para construir y desplegar **aplicaciones web altamente escalables**.
*   **Características integradas:** Balanceo de carga automático, control de versiones de la app y división de tráfico (*traffic splitting*).
*   **Uso ideal:** Equipos que ya están familiarizados con los flujos de trabajo de App Engine o que tienen aplicaciones heredadas (*legacy*) que necesitan mantener.

---

## 3. Beneficios Estratégicos y de Negocio (Clave para el Examen)

La adopción de Serverless no es solo un cambio técnico, sino una decisión financiera y operativa estratégica:

*   **Precios por uso real (Pay-per-use):** Cero costo por tiempo de inactividad. Solo pagas por los recursos de cómputo exactos que utilizas mientras el código se está ejecutando.
*   **Costos operativos reducidos:** Google maneja el mantenimiento, parches de seguridad y actualizaciones de hardware. Menos carga para el equipo de TI.
*   **Escalabilidad instantánea:** Los recursos suben o bajan en tiempo real según la demanda, eliminando la necesidad de planificar la capacidad de los servidores (*capacity planning*).
*   **Menor tiempo de comercialización (Faster time-to-market):** Los desarrolladores se enfocan 100% en la lógica del negocio y el código, no en configurar infraestructura, acelerando el lanzamiento de nuevas funciones.
*   **Resiliencia mejorada:** Google Cloud gestiona automáticamente la recuperación ante desastres (*disaster recovery*) y la tolerancia a fallos.

---

##  Enfoque de Negocio (Toma de Decisiones para el Examen)

*   **¿Quieres desplegar una aplicación web en un contenedor sin administrar servidores y que no cobre nada si no hay tráfico?** ➡️ **Cloud Run**.
*   **¿Necesitas ejecutar un fragmento de código pequeño solo cuando ocurra una acción específica (como subir una foto)?** ➡️ **Cloud Run Functions**.
*   **¿Buscas una plataforma web que administre automáticamente versiones de la app y divida el tráfico entre ellas?** ➡️ **App Engine**.