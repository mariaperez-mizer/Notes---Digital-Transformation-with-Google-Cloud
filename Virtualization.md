## 1. Virtualización y Compute Engine (IaaS)

La **virtualización** es una forma de optimización de recursos que permite que múltiples sistemas operativos e instrucciones corran en el mismo hardware físico. Estos sistemas aislados se conocen como **Máquinas Virtuales (VMs)** y comparten un mismo *pool* de procesamiento (CPU), memoria, almacenamiento y red.

**Compute Engine** es el producto de **Infraestructura como Servicio (IaaS)** de Google Cloud que te permite crear y administrar estas VMs en la infraestructura de Google, sin inversiones iniciales (*no upfront investments*) y pagando solo por segundo (con un mínimo de 1 minuto).

> [!NOTE] ¿Cómo se crean las VMs?
> Se pueden crear manualmente desde la **Consola web** o la **Google Cloud CLI**. Para automatizar el proceso como código, se utilizan herramientas de infraestructura como **Terraform** o la **Compute Engine API** (diseñada específicamente para la gestión de infraestructura, no para comunicación de aplicaciones).

### 🎛️ Tipos de Instancias y Precios (Estrategia de Costos)
Puedes elegir propiedades de máquina predefinidas o crear **custom machine types** (personalizadas). Google ofrece tres modelos de descuento clave para el examen:

*   **Sustained-use discounts (Descuentos por uso continuo):** Se aplican **automáticamente** si una VM corre por más del 25% del mes. No requiere contratos ni configuración previa.
*   **Committed-use discounts (CUDs - Descuentos por uso comprometido):** Requieren un compromiso de compra de **1 o 3 años**. Ideal para cargas de trabajo predecibles y estables. Ofrece grandes descuentos sobre el precio bajo demanda.
*   **Spot VMs:** Ofrecen hasta un **91% de descuento**. La única diferencia es que Google puede **interrumpirlas (preemptively interrupt)** en cualquier momento si necesita la capacidad. Ideal para tareas por lotes (*batch jobs*) o análisis de datos donde si el proceso se detiene, se puede reiniciar después sin impacto negativo.

---

## 2. Contenedores y Microservicios

Mientras que las VMs virtualizan el *hardware* (mediante un **Hypervisor**), los **contenedores** virtualizan el *sistema operativo*. Un contenedor empaqueta la aplicación junto con todas sus dependencias para garantizar que corra de forma idéntica en cualquier entorno.

| Característica | Máquinas Virtuales (VMs) | Contenedores |
| :--- | :--- | :--- |
| **Enfoque** | Virtualiza el **Hardware** | Virtualiza el **Software / OS** |
| **Componente clave** | Hypervisor + Sistema Operativo completo | Motor de contenedores (Comparte el OS del Host) |
| **Eficiencia** | Más pesadas, tardan minutos en arrancar | Ligeras, arrancan en segundos, usan menos memoria |
| **Arquitectura típica**| Aplicaciones monolíticas tradicionales | Microservicios, portabilidad extrema |

> [!TIP] Examen: Arquitectura de Microservicios
> Los contenedores facilitan dividir una aplicación grande en componentes pequeños e independientes (**Microservicios**) que se comunican entre sí mediante **APIs** (como REST o gRPC). Esto permite actualizar una sola parte de la app sin romper el resto, mejorando la agilidad.

---

## 3. Orquestación de Contenedores: GKE vs. Cloud Run

Cuando manejas millones de contenedores a escala, necesitas un orquestador. **Kubernetes** es la plataforma *open-source* (creada originalmente por Google) para automatizar el despliegue, escalado y gestión de contenedores.

Google Cloud ofrece dos servicios principales para esto, dependiendo del nivel de control que necesites:

### A) Google Kubernetes Engine (GKE)
Es el servicio administrado de Kubernetes en Google Cloud. Corre sobre grupos de instancias de Compute Engine (llamados *clusters*).
*   **GKE Autopilot:** Es un modo de operación donde Google administra **toda** la infraestructura del cluster (nodos, seguridad, actualizaciones). Tú solo te preocupas por tus aplicaciones y Google te cobra **por Pod activo** (*per-Pod billing*). *(Caso de estudio: La startup Ubie redujo 20% sus costos de infraestructura y eliminó días de mantenimiento usando Autopilot).*

### B) Cloud Run
Es una plataforma **totalmente administrada y Serverless** para ejecutar contenedores.
*   **Cómo funciona:** Subes tu código o contenedor y Google se encarga de todo el escalado de forma automática (incluso escala a **cero** si no hay tráfico, por lo que no pagas nada).
*   **Ideal para:** Aplicaciones ligeras, sin estado (*stateless*), como aplicaciones web que necesitan reaccionar rápidamente a picos de tráfico.

---

## Enfoque de Negocio (Toma de Decisiones para el Examen)

Para el examen de *Digital Leader*, la clave es saber **qué servicio elegir** según la necesidad del negocio:

*   **¿Necesitas migrar una app vieja tal cual está (Lift-and-Shift) con acceso total al OS?** ➡️ **Compute Engine (VMs)**.
*   **¿Quieres ahorrar hasta un 91% en un proceso de datos que puede pausarse?** ➡️ **Spot VMs**.
*   **¿Necesitas máximo control, configuraciones de red personalizadas y arquitectura compleja de contenedores?** ➡️ **GKE (Standard)**.
*   **¿Quieres contenedores pero CERO administración de servidores y pagar solo por Pod ejecutado?** ➡️ **GKE Autopilot**.
*   **¿Quieres desplegar una app web rápido, sin configurar infraestructura y que escale a cero si no hay visitas?** ➡️ **Cloud Run (Serverless)**.