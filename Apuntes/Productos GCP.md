## 1. Cómputo (Compute)

Son los servicios destinados a procesar datos y ejecutar aplicaciones.

- **Compute Engine:** Máquinas virtuales (VMs) en la nube. Es **Infraestructura como Servicio (IaaS)**; tú eliges el sistema operativo y el tamaño del servidor.
    
- **Google Kubernetes Engine (GKE):** Servicio gestionado para ejecutar contenedores utilizando Kubernetes. Ideal para aplicaciones modernas que necesitan escalar automáticamente.
    
- **Cloud Run:** Plataforma **Serverless** (sin servidor) para ejecutar contenedores. La infraestructura se gestiona sola y solo pagas por los segundos exactos en que tu código se está ejecutando.
    
- **App Engine:** Plataforma como Servicio (PaaS). Los desarrolladores solo suben su código (web o móvil) y Google se encarga de todo lo demás (redes, servidores, escalabilidad).
    
- **Google Cloud VMware Engine / Bare Metal:** Permiten migrar servidores tradicionales o entornos VMware existentes directamente a la nube de Google sin tener que rediseñar la aplicación.
    

## 2. Almacenamiento y Bases de Datos (Storage & Databases)

Dónde se guardan los datos, dependiendo de su formato y uso.

- **Cloud Storage:** Almacenamiento de objetos (fotos, videos, respaldos). Ofrece diferentes "clases" según qué tan seguido accedas a los datos (**Standard, Nearline, Coldline y Archive**), lo que ayuda a optimizar costos.
    
- **Cloud SQL:** Base de datos relacional (SQL) completamente gestionada (compatible con MySQL, PostgreSQL y SQL Server). Ideal para sistemas tradicionales o de comercio electrónico.
    
- **Cloud Spanner:** Base de datos relacional a **escala global**. Combina los beneficios de SQL con una escalabilidad horizontal masiva. Diseñada para bancos o empresas globales que no pueden permitirse ni un segundo de caída.
    
- **Cloud Bigtable:** Base de datos NoSQL diseñada para manejar volúmenes masivos de datos analíticos con lecturas y escrituras ultrarrápidas (ideal para datos de IoT o financieros).
    
- **Firestore:** Base de datos NoSQL orientada a documentos, excelente para aplicaciones web y móviles que requieren sincronización de datos en tiempo real.
    

## 3. Analítica de Datos y Big Data

Herramientas para procesar datos y extraer información valiosa para el negocio.

- **BigQuery:** El almacén de datos (**Data Warehouse**) empresarial de Google. Es serverless y te permite analizar petabytes de datos en segundos usando comandos SQL tradicionales. Es el producto estrella de analítica en el examen.
    
- **Pub/Sub:** Servicio de mensajería que permite conectar aplicaciones independientes y recibir flujos de datos en tiempo real (ingesta de datos).
    
- **Dataflow:** Procesa y transforma datos en tiempo real (streaming) o en lotes (batch). Automatiza los flujos de preparación de datos antes de analizarlos.
    
- **Dataproc:** Servicio gestionado para ejecutar herramientas de código abierto como Apache Spark y Hadoop. Sirve para empresas que ya tienen infraestructura de Big Data antigua y quieren moverla a la nube.
    
- **Looker:** Plataforma de Inteligencia de Negocio (BI) para crear dashboards, reportes visuales y gráficos interactivos basados en los datos de la empresa.
    

## 4. Inteligencia Artificial y Machine Learning (AI & ML)

Servicios para automatizar procesos y generar innovación con modelos inteligentes.

- **Vertex AI:** La plataforma unificada de Google Cloud para construir, entrenar y desplegar modelos de IA. Incluye acceso a herramientas de IA generativa (como **Gemini**).
    
- **APIs de IA preentrenadas (Vision, Natural Language, Translation, Speech-to-Text):** Modelos listos para usar mediante programación sencilla. Permiten a una empresa añadir reconocimiento de imágenes o traducción de idiomas a sus apps sin necesidad de científicos de datos.
    

## 5. Modernización de Aplicaciones y Redes (Networking & Modernization)

Cómo se conectan los sistemas y cómo se abren al mundo.

- **Apigee:** Plataforma de gestión de APIs. Permite a las empresas conectar sus sistemas internos con aplicaciones de terceros, socios comerciales o clientes de forma segura y controlada.
    
- **AppSheet:** Plataforma **No-Code** (sin código) que permite a cualquier empleado crear aplicaciones móviles o web para automatizar tareas internas usando datos de hojas de cálculo u otras fuentes.
    
- **GKE Enterprise (antes Anthos):** Plataforma para gestionar aplicaciones de forma consistente tanto en centros de datos propios (**On-Premise**) como en múltiples nubes (**Multi-cloud**).
    
- **VPC (Virtual Private Cloud):** La red virtual privada de la empresa dentro de Google Cloud para conectar todos sus recursos de forma segura.
    
- **Cloud Load Balancing:** Balanceador de carga que distribuye el tráfico web de los usuarios para asegurar que las aplicaciones no se saturen y siempre respondan rápido.
    

## 6. Seguridad, Operaciones y Finanzas

Herramientas para mantener el control, la salud de la plataforma y el presupuesto.

- **IAM (Identity and Access Management):** Control de acceso que define exactamente **quién** tiene permiso para hacer **qué** en **cuál** recurso. Aplica el "principio del menor privilegio".
    
- **Cloud Operations Suite (antes Stackdriver):** Incluye **Cloud Monitoring** (para ver el rendimiento y salud del sistema) y **Cloud Logging** (el historial o bitácora de todo lo que ocurre).
    
- **Google Cloud Billing:** Herramientas para monitorear el gasto, configurar alertas de presupuesto y optimizar los costos de la nube (conceptos clave de **FinOps**).