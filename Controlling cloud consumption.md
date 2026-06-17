

---

## 1. El Control del Consumo: Proactivo vs. Reactivo

Una vez que la jerarquía de recursos está bien estructurada y los accesos están seguros, el siguiente paso estratégico es la **optimización del consumo**. Controlar el gasto en la nube no solo evita sorpresas financieras, sino que maximiza el valor de la inversión, mejora la visibilidad entre departamentos y asegura el cumplimiento regulatorio.

Para el examen, las herramientas de control se dividen en dos enfoques: **Proactivas** (evitan el gasto antes de que ocurra) y **Reactivas** (analizan el gasto que ya ocurrió).

> [!NOTE] Sabiduría de la Nube
> Como dicen Katelyn y Joe: *"La única fiesta peor que una fiesta sorpresa es una factura sorpresa de la nube"*. Pasar de la simple gestión a la optimización requiere combinar ambas estrategias.

---

## 2. Caja de Herramientas para Controlar el Consumo

Google Cloud ofrece seis herramientas clave que debes conocer a fondo para responder los casos prácticos del examen:

###  Herramientas Proactivas (Prevención y Alertas)
*   **Políticas de Cuotas de Recursos (Resource Quota Policies):** Permiten establecer límites duros en la cantidad de recursos que un proyecto o un usuario específico puede consumir (ej. limitar a máximo 5 VMs en un proyecto de prueba). Evitan el sobregasto deteniendo el aprovisionamiento excesivo. Se configuran en la consola.
*   **Reglas de Umbral de Presupuesto (Budget Threshold Rules):** Permiten configurar alertas automáticas para notificar al equipo (y a Finanzas) mediante correo cuando los costos reales o **pronosticados (*forecasted*)** superan un porcentaje o monto específico. Funcionan como una alarma temprana antes de que el presupuesto se salga de control.

###  Herramientas Reactivas e Históricas (Análisis de Datos)
*   **Informes de Facturación de Cloud (Cloud Billing Reports):** Permiten monitorear y desglosar los costos que la empresa ya generó. Para análisis masivos y avanzados de tendencias entre departamentos, estos datos se pueden **exportar a BigQuery** y visualizarse en herramientas como Looker Studio (Data Studio).

###  Herramientas de Optimización y Descuentos
*   **Programador Dinámico de Cargas de Trabajo (Dynamic Workload Scheduler):** Diseñado para cargas de trabajo que no son urgentes. Permite programar el uso de recursos por una duración predeterminada a una tarifa con descuento. *Ejemplo de negocio:* Apagar automáticamente los entornos de desarrollo durante la noche y fines de semana cuando nadie trabaja.
*   **Spot VMs:** Utilizan la capacidad ociosa de Compute Engine con hasta un **91% de descuento**. Son interrumpibles (Google las reclama con un aviso de 30 segundos). Ideales para tareas tolerantes a fallos como procesamiento de datos por lotes (*batch processing*) o pruebas.
*   **Descuentos por Uso Comprometido (CUDs):** Descuentos masivos a cambio de comprometerse por contrato a un consumo mínimo de recursos durante un término de **1 o 3 años**. Ideal para cargas de trabajo estables y predecibles.

---

## Enfoque de Negocio (Toma de Decisiones para el Examen)

*   **¿Qué herramienta debes configurar para recibir un correo de advertencia cuando tu proyecto gaste el 80% del dinero asignado?** ➡️ **Budget Threshold Rules** (Reglas de umbral de presupuesto).
*   **¿Cómo puede una empresa multinacional analizar a detalle qué departamentos están gastando más y crear páneles visuales de sus tendencias de facturación?** ➡️ Exportando los **Cloud Billing Reports a BigQuery** y visualizándolos con Looker Studio / Data Studio.
*   **¿Qué solución técnica reduce costos al apagar servidores de prueba que solo se necesitan en horario laboral?** ➡️ **Dynamic Workload Scheduler** (Programador de cargas de trabajo).
*   **¿Qué mecanismo evita físicamente que un desarrollador cree por error 100 bases de datos gigantes en un proyecto de práctica?** ➡️ **Resource Quota Policies** (Políticas de cuotas de recursos).
*   **¿Cuál es la mejor opción para ahorrar dinero en una carga de trabajo cuyo consumo de servidores es exactamente el mismo todos los meses del año?** ➡️ Comprar **Committed Use Discounts (CUDs)**.