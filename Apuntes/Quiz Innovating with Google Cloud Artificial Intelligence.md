1. Una compañía de seguros ha desarrollado un modelo Python personalizado para la detección de fraudes. Necesitan una plataforma unificada de Google Cloud para gestionar sin problemas el entrenamiento, la implementación, la monitorización en tiempo real y el reentrenamiento automático del modelo en un único entorno integrado. ¿Qué oferta de Google Cloud es la más adecuada para gestionar todo este ciclo de vida del aprendizaje automático personalizado?

     
   Agent Studio on Gemini Enterprise Agent Platform


2. Un importante centro de llamadas está siendo sometido a una auditoría de control de calidad y cumplimiento normativo. El centro necesita convertir automáticamente miles de llamadas de atención al cliente grabadas en transcripciones de texto con capacidad de búsqueda. ¿Qué API preentrenada de Google Cloud es la más adecuada para esta tarea específica?

   Speech-to-Text API

3.   Una empresa de moda quiere crear un modelo de aprendizaje automático que identifique su línea de ropa de primavera a partir de fotos subidas por los clientes. El equipo de marketing tiene miles de imágenes etiquetadas de sus productos, pero carece de conocimientos de programación y experiencia en ciencia de datos. ¿Qué solución de Google Cloud les permite entrenar y personalizar este modelo sin escribir código?

     AutoML en Agent Studio en la plataforma Gemini Enterprise Agent

4. Entrenar un modelo de IA generativa masivo requiere que miles de procesadores funcionen como una supercomputadora. ¿Qué componente central de la hipercomputadora de IA garantiza que estos procesadores puedan compartir datos masivos de manera eficiente?

   La red dedicada de alto rendimiento construida específicamente para GPU y TPU.

5. Un equipo experto en aprendizaje automático quiere crear un modelo de visión artificial para detectar defectos de propiedad intelectual y obtener una ventaja competitiva. ¿Qué solución de Google Cloud ML se ajusta mejor a este objetivo estratégico?

   Modelos personalizados creados en Agent Studio en la plataforma Gemini Enterprise Agent.

6. Un analista necesita crear rápidamente un modelo predictivo utilizando SQL sobre grandes volúmenes de datos de BigQuery, pero carece de conocimientos de Python. ¿Qué funcionalidad principal de BigQuery ML permite esta capacidad?

   La capacidad de crear y ejecutar el modelo de aprendizaje automático directamente mediante consultas SQL estándar.


---

Respuestas 3 y 5

### 3
## El equipo de marketing y la línea de ropa

> **El escenario:** Un equipo de marketing **sin conocimientos de programación** quiere identificar su línea de ropa específica usando **miles de imágenes ya etiquetadas** por ellos.
> 
> **Respuesta correcta:** AutoML en Agent Studio en la plataforma Gemini Enterprise Agent.

### ¿Por qué esta es la respuesta?

- **La pista clave:** _"Carece de conocimientos de programación"_ + _"Tiene imágenes etiquetadas"_.
    
- **Por qué es AutoML:** **AutoML** (Automatic Machine Learning) es la herramienta de Google diseñada específicamente para personas que **no saben programar**, pero que tienen sus propios datos. Tú solo subes las fotos de tu ropa de primavera, le dices a la plataforma qué es cada cosa, y el sistema genera un modelo personalizado de forma automática.
    
- **Por qué NO son las otras:**
    
    - **API de visión preentrenada:** Las APIs preentrenadas son geniales y no requieren código, pero **ya vienen enseñadas por Google**. Si le subes una foto de tu ropa, la API te dirá: _"Es un vestido azul"_, pero nunca sabrá que es el _"Vestido Primavera Modelo 2026 de tu marca"_, porque Google no conoce tus productos.
        
    - **BigQuery ML:** Esto se usa para hacer modelos predictivos usando tablas de datos y lenguaje SQL (como bases de datos), no para reconocimiento de imágenes de clientes.


### 5
## El equipo experto y los defectos de propiedad intelectual

> **El escenario:** Un **equipo experto** en ML quiere detectar defectos muy específicos para obtener una **ventaja competitiva** en el mercado. **Respuesta correcta:** Modelos personalizados creados en Agent Studio en la plataforma Gemini Enterprise Agent.

### ¿Por qué esta es la respuesta?

- **La pista clave:** _"Equipo experto"_ + _"Ventaja competitiva"_.
    
- **Por qué son Modelos Personalizados (Custom Training):** Cuando un equipo es experto, no quiere que Google haga todo en automático (como con AutoML). Ellos quieren escribir su propio código, ajustar los algoritmos matemáticos a mano y diseñar una IA única desde cero. Esto es lo que les da la **ventaja competitiva**, porque crean una tecnología patentada que ninguna otra empresa tiene.
    
- **Por qué NO son las otras:**
    
    - **Soluciones de bajo código / APIs preentrenadas:** Sería un desperdicio para un equipo experto. Además, las herramientas genéricas o de bajo código las puede usar cualquier competidor, por lo que no te darían una ventaja estratégica real en el mercado para detectar algo tan exclusivo como "defectos de propiedad intelectual".