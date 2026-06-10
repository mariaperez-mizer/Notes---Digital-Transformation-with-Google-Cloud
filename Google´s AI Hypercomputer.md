
Un sistema  que combina computación especializada, redes, almacenamiento y software para maximizar el rendimiento y la eficiencia de estas cargas de trabajo intensivas.

Google Cloud ofrece dos opciones: 
- GPU( Unidades de Procesamiento Gráfico) NVIDIA, que son versátiles y flexibles.
	- Procesadores paralelos
- Unidades de Procesamiento Tensorial (TPU), diseñadas a medida por Google específicamente para acelerar el aprendizaje profundo.
	- optimizadas para las multiplicaciones de matrices masivas necesarias para el entrenamiento de redes neuronales profundas.
	- Velocidad y rentabilidad para tareas de entrenamiento e inferencia a gran escala

- Integra este hardware personalizado con marcos de código abierto para automatizar tareas complejas en miles de procesadores interconectados.

--- 

#### Beneficios

- **Open-source compatibility**  Totalmente compatible con frameworks populares como PyTorch, JAX y TensorFlow, lo que permite a los desarrolladores usar código conocido.

- **Proprietary orchestration** Los frameworks propietarios de Google, como Pathways on Cloud, gestionan todo el sistema.

- **Automated deployment** Aprovecha Google Kubernetes Engine (GKE), basado en Kubernetes, un potente estándar abierto para automatizar la implementación, el escalado y la gestión de aplicaciones en contenedores.

### Ventajas

- Mayor flexibilidad 
	- Google ofrece soporte nativo para los frameworks de código abierto que los equipos ya utilizan, como TensorFlow, PyTorch y JAX.
	
- Máxima optimización del presupuesto
	- Pago por uso, descuentos por uso comprometido y reservas para garantizar que tengas la capacidad cuando la necesites.
- Spot VMs ofrecen grandes descuentos y son ideales para cargas de trabajo donde la tolerancia a fallos está integrada en el software, lo que permite que incluso las tareas críticas de aprendizaje automático se ejecuten en capacidad interrumpible.