Estrategia de migración a la nube (Rehosting).

---
##### ¿ En qué consiste ?

Copia una aplicación y sus datos exactamente como están on-premises y los mueve a la nube, esto es , sin realizar *ningún cambio* en el código ni en la arquitectura de la aplicación.

##### ¿ En Google Cloud?

Del servidor físico de una oficina, se aplica lift and shift, y el usuario crea una máquina virtual idéntica en la nube (con Compute Engine de Google Cloud) y clona el sistema ahí.

---
##### Ventajas

1. Migración más rápida y fácil : pasas de meses a , semanas incluso días.
2. Menor riesgo: Esto se debe a que no se modifica el código.
3. Reducción de costos inmediatos: Permite cerrar centros de datos físicos con rapidez.

##### Desventajas

1. Desaprovechamiento del potencial de la nube: La aplicación funcionara exactamente igual que cuando estaba on-premises.
2. No es "Cloud-Native": No se pueden aprovechar herramientas automáticas como "auto-escalado" o bases de datos autoadministradas.


>[!important] Es la forma más rápida y menos disruptiva de migrar a la nube, pero es solo el primer paso antes de optimizar las aplicaciones más adelante.

