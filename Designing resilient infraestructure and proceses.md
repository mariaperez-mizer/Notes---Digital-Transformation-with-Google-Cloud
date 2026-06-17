
---

## 1. Diseño de Infraestructura Resiliente

La **confiabilidad** no es algo que se "compra", es algo que se **diseña**. Para cumplir con tus objetivos de nivel de servicio (SLOs), debes construir sistemas que anticipen la falla.

### Conceptos Clave de Resiliencia:
* **Alta Disponibilidad (HA):** Capacidad del sistema de permanecer operativo incluso ante fallas de hardware o software.
* **Recuperación ante Desastres (DR):** Proceso de restaurar el sistema a un estado funcional tras una catástrofe mayor.
* **Redundancia:** Duplicar componentes críticos (fuentes de poder, balanceadores, switches) para que, si uno falla, otro tome el control instantáneamente sin que el usuario lo note.
* **Replicación:** Crear copias de datos o servicios en diferentes ubicaciones físicas.
    * **Zonas:** Ubicaciones aisladas dentro de una misma región. Protegen contra la falla de un centro de datos.
    * **Regiones:** Áreas geográficas distintas. Protegen contra desastres naturales o problemas de red que afecten a toda una zona geográfica.
* **Escalamiento Automático (Autoscaling):** Capacidad dinámica de asignar o liberar recursos según la demanda. Mantiene la disponibilidad durante picos de tráfico y optimiza costos durante los valles.
* **Copias de Seguridad (Backups):** Deben almacenarse en **ubicaciones geográficamente separadas** de la fuente original para garantizar la recuperación ante un desastre regional.

[Image of Google Cloud regions and zones architecture]

---

## 2. Gestión de Trade-offs: ¿Cuánta fiabilidad es suficiente?

No toda aplicación necesita ser "a prueba de balas". La ingeniería de confiabilidad es una gestión de equilibrios:

* **El "Impuesto de Consistencia":** Replicar datos de forma síncrona en todo el mundo puede garantizar que todos vean lo mismo al mismo tiempo, pero **aumenta la latencia**. Si la aplicación no lo necesita, estás pagando un precio alto en velocidad por una confiabilidad que el negocio no requiere.
*