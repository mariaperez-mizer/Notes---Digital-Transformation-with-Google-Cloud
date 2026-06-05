
----
##### Base de datos

Colección organizada de datos almacenados en tablas y a la que se accede electrónicamente desde un sistema informático.

- Relacionales: Almacena y proporciona acceso a puntos de datos que están relacionados entre sí.
	- Altamente consistentes, fiables y la más adecuada para gestionar grandes cantidades de **datos estructurados**.
	
- No relacionales: Siguen un modelo de datos flexible.
	- Datos cuya organización cambia con frecuencia.
	- Apps con diversos tipos de datos.
	- No grandes cantidades de datos complejos o diversos
	- No cuando los datos evolucionan periódicamente

---
##### Data warehouses

Esta diseñado para analizar datos y la elaboración de informes de datos estructurados y semiestructurados procedentes de múltiples fuentes.

- Puntos de venta
- Automatización de marketing
- Datos de CRM

Datos previamente procesados y limpios.
Usuarios: Analistas de inteligencia empresarial,  

---
##### Data lakes

Es un repositorio diseñado para ingerir, almacenar, explorar, procesar y analizar cualquier tipo o volumen de datos sin procesar, independientemente de su origen, por ejemplo:
- Sistemas operativos 
- Fuentes web
- Redes sociales
- IoT
Puede almacenar diferentes tipos de datos en su tamaño original; ignorando los limites de tamaño.
- Evita contaminación involuntaria de los datos.
- Introducción de sesgos.
- Combinación de datos simultaneamente.

Usuarios: Ingenieros de datos, científicos de datos

---
### Productos de Google Cloud

1. Cloud SQL y Spanner para Bases de datos relacionales.
2. Bigtable para Bases de datos no relacionales.
3. BigQuery para Data warehouses estructurados y semi-estructurados.

Para Data lake con datos estructurados:
1. Cloud SQL 
2. Spanner
3. BigQuery 

Para Data lake con datos semi-estructurados:
1. Datastore
2. Bigtable

Para Data lake con datos no estructurados:
1. Cloud Storage