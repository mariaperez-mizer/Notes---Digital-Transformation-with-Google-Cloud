
Almacenamiento de objetos: es una arquitectura de almacenamiento de datos informáticos que gestiona los datos como *objetos* en lugar de como almacenamiento de archivos (una jerarquía de archivos y carpetas) o como almacenamiento de bloques (fragmentos de un disco).
	 *Forma binaria de los datos reales.*

Datos no estructurados
- Vídeos
- Imágenes 
- Grabaciones de audio.

---

### Productos de Google

1. Cloud Storage, un servicio que ofrece a desarrolladores y organizaciones de TI almacenamiento de objetos duradero y de alta disponibilidad.
	1. Standard Storage se considera ideal para datos de acceso frecuente, también es excelente para datos que se almacenan solo por períodos breves.
	2. Nearline Storace: Almacenar datos de acceso poco frecuente: como datos que se leen o modifican en promedio una vez al mes o menos.
		- Copias de seguridad de datos
		- Contenido multimedia de baja frecuencia
		- Archivado de datos.
	3. Coldline Storace: Opción económica para almacenar datos de acceso poco frecuente. Está diseñado para leer o modificar datos, como máximo, una vez cada 90 días.
	4. Archive Storage: Es la opción de menor costo, ideal para archivar datos, realizar copias de seguridad en línea y recuperarse de desastres.
	     - Acceder menos de una vez al año.
	     - Costos altos de acceso y operación de datos
	     - Una duración mínima de almacenamiento de 365 días.
Todas:
- Almacenamiento ilimitado sin requisito de tamaño mínimo de objeto
- Accesibilidad y ubicaciones a nivel mundial
- Baja latencia y alta durabilidad
- Experiencia uniforme (que se extiende a la seguridad, las herramientas y las API)
- Geo-redundacy si los datos se almacenan en una región múltiple o dual.


Ofrece una función llamada **Autoclass**, que clasifica automáticamente los objetos en las clases de almacenamiento adecuadas según su patrón de acceso.
- Simplifica y automatiza el ahorro de costes para sus datos de almacenamiento en la nube.