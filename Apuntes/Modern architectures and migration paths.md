
---

## 1. Monolitos vs. Microservicios (Desarrollo Moderno)

En el modelo tradicional local (*on-premises*), las aplicaciones se desarrollaban como **Monolitos** (un solo bloque masivo de código). Implementar cambios en este modelo requería meses de planeación y ponía en riesgo a todo el sistema. 

El desarrollo moderno en la nube migra hacia una arquitectura de **Microservicios**.

> [!NOTE] La analogía de los bloques de LEGO
> Piensa en los microservicios como piezas de LEGO. La aplicación se divide en componentes independientes. Si una sección de la app tiene un pico de tráfico (por ejemplo, el carrito de compras), no necesitas duplicar todo el castillo (toda la app); solo agregas más bloques a la torre que lo necesita (escalado eficiente bajo demanda).

### 🚀 Beneficios del Desarrollo Nativo de la Nube
*   **Servicios Administrados (Managed Services):** Google se encarga del mantenimiento rutinario (actualizaciones, parches de seguridad, monitoreo). Esto libera a los desarrolladores para enfocarse en innovar y crear código, no en "mantener las luces encendidas".
*   **Balanceo de Carga (Load Balancing):** Actúa como un "oficial de tránsito" que distribuye el tráfico web de forma equitativa entre los servidores para que la app no se caiga.
*   **Conmutación por error automática (Automatic Failover):** Si un servidor falla, el sistema lo detecta al instante y redirige el tráfico a un respaldo. El sistema "se sana a sí mismo" sin que el usuario lo note.

---

## 2. Estrategia de Migración: Rehost (Lift and Shift)

Reconstruir una aplicación desde cero para que sea nativa de la nube no siempre es realista a corto plazo, especialmente si es software heredado (*legacy*). Para esto se usa la estrategia de **Rehost** o **Lift and Shift** (Levantar y Mudar).

*   **¿Qué es?** Mover una aplicación desde el entorno local a la nube **sin realizar ningún cambio en su código** o arquitectura.
*   **Ventajas:** Es una forma rápida de obtener beneficios de la nube (seguridad, escalabilidad básica, reducción de costos físicos).
*   **Desventajas / Riesgos para el examen:** Requiere planeación cuidadosa y existe el riesgo de **dependencia del proveedor (vendor lock-in)**, ya que adaptas la infraestructura al proveedor elegido y podría ser difícil cambiar después.

---

## 3. Rutas de Migración Especializadas de Google Cloud

Cuando las aplicaciones heredadas son muy complejas o corren en plataformas específicas, Google Cloud ofrece dos soluciones de infraestructura dedicada para hacer el *Lift and Shift*:

### A) Google Cloud VMware Engine (GCVE)
Permite migrar cargas de trabajo de **VMware** existentes a la nube de Google **sin rediseñar las aplicaciones** ni cambiar la forma en que opera el equipo de TI.
*   **Beneficio clave:** Mantienes tu entorno VMware tal como lo conoces, pero ganas la confiabilidad de Google y acceso inmediato a servicios nativos avanzados como BigQuery (analítica) e Inteligencia Artificial (AI/ML).

### B) Bare Metal Solution (Solución de Servidor Físico/Puro)
Diseñada para aplicaciones tradicionales ultraespecializadas (como bases de datos **Oracle**) que no se pueden virtualizar fácilmente o que requieren un rendimiento físico bruto.
*   **Beneficio clave:** Google te proporciona servidores físicos dedicados (sin capas de virtualización) con altísimo rendimiento y baja latencia, manteniendo intactos tus procesos operativos y licencias actuales.

---

## 🎯 Enfoque de Negocio (Toma de Decisiones para el Examen)

*   **¿El cliente quiere migrar rápido a la nube sin tocar ni una sola línea de código de su app?** ➡️ Estrategia **Rehost / Lift and Shift**.
*   **¿La empresa usa entornos de VMware y quiere moverlos a la nube sin cambiar sus herramientas de operación actuales?** ➡️ **Google Cloud VMware Engine**.
*   **¿El examen menciona bases de datos especializadas (como Oracle) que no se pueden virtualizar y requieren hardware físico dedicado?** ➡️ **Bare Metal Solution**.