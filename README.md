# Proyecto de evaluación

---

<div style="text-align: center;">
    <img src="https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExbjZxaG9sMzFscnZ4a2Vkc2pxbWd3Y3g2eTNweDI2anNteXlidDdlNiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/doXBzUFJRxpaUbuaqz/giphy.webp" alt="Data Ana">
</div>

---

## Autor: Juan Carlos González Ibarra
## Correo Institucional: juan.gonzalez.dti@imfe.mx

---

## Fecha: 17 de junio, 2023

---

## Contenido

1. Introducción
2. Objetivo
3. Descripción del Tema de Tesis
4. Metodología de Desarrollo
5. Data Clean
6. Análisis exploratorio de Datos (AED)
7. Resultados de AED
8. Modelado de Datos
9. Conclusión

---
# 1. Introducción

La tecnología está presente cada vez más en nuestras vidas, podemos notarlo de tal forma que nuestras actividades diarias están vinculadas a compartir información por medios digitales, sin duda esto hace que la información recolectada por estos medios digitales sea visualizada como una herramienta en la toma de decisiones y/o en la solución de problemas. Esta información para poder ser utilizada con estos propósitos previamente debe haber pasado por un proceso de análisis; este proceso de análisis ya tiene una base científica y aplicativa llamada ciencia de datos. La ciencia de datos conlleva una serie de etapas para el análisis de la información como: el entendimiento de los datos, la extracción de sus propiedades, el modelado y análisis del problema, la presentación de resultados y el desarrollo de software para explotar el conocimiento extraído. La **Ciencia de Datos** proporciona las herramientas y en ayuda del **Big Data** provee nuevas oportunidades tecnológicas para análisis masivos de información, por lo que las Tecnologías Big Data ayudan a mejorar la eficiencia, calidad y los productos y servicios personalizados ofrecidos por las organizaciones y a integrar datos estructurados y no estructurados con respuestas en tiempo real, abriendo nuevos caminos a la innovación y desarrollo.


Por lo que el **Big Data** se refiere al manejo y análisis de enormes volúmenes de datos que no pueden ser procesados de manera efectiva con las técnicas tradicionales debido a su volumen, velocidad y variedad. Los datos pueden provenir de varias fuentes, como transacciones comerciales, sensores de IoT, redes sociales, datos de salud, etc. Las técnicas de Big Data permiten descubrir patrones ocultos, correlaciones y otras ideas útiles que pueden informar la toma de decisiones empresariales y estratégicas.

Por lo que para realizar este análisis masivo de datos se debe identificar patrones que ayuden a la toma de decisiones tenemos que llevar acabo el **Análisis Exploratorio de Datos (AED)**.


## 1.1 Análisis Exploratorio de Datos
Se utiliza para analizar e investigar conjuntos de datos y resumir sus características principales, a menudo empleando métodos de visualización de datos que ayuda a entender la estructura de estos. Es un paso crucial antes de realizar modelos más complejos ya que ayuda a gestionar las fuentes de datos, descubrir patrones, detectar anomalías, probar una hipótesis, identificar relaciones y tendencias, etc.

<img src="https://datos.gob.es/sites/default/files/u322/grafico-guia_0.jpg" width="600" height="400">

El **AED** es un paso esencial en cualquier flujo de trabajo de **análisis de datos**, implica el uso de algoritmos de muestreo y agregación para reducir la escala de los datos a un tamaño manejable, y luego explorar estos datos resumidos para obtener insights. 
 
Source: https://www.ibm.com/mx-es/topics/exploratory-data-analysis

El **AED** forma parte de cualquier **metodología para el análisis de datos**. Es una fase inicial en la que los analistas examinan los datos para comprender sus características principales antes de aplicar modelos más complejos. Aquí es cómo el AED se vincula con una metodología general para el **análisis de datos**.

## 1.2 Metodología en el Análisis de Datos
  
Para establecer una metodología en el análisis de datos, debemos definir que el análisis de datos es el proceso de convertir datos sin procesar en información práctica e incluye una serie de herramientas, tecnologías y procesos para encontrar tendencias y resolver problemas mediante datos.

Source: https://aws.amazon.com/es/what-is/data-analytics/

<img src="https://actions.es/wp-content/uploads/2020/08/datos1-1.jpg" width="600" height="400">


Existen metodologías para el análisis de datos, en esta guía básica realizada por Non-Profit Evaluation & Resource Center, Inc. (NPERCI) presenta los pasos generales para procesar y analizar datos.

Definición del problema: Antes de comenzar cualquier análisis, es crucial definir claramente el problema que se está tratando de resolver. Esto implica entender el contexto del problema y los objetivos del análisis.

Recolección de datos: Una vez definido el problema, el siguiente paso es recoger los datos necesarios para el análisis. Esto puede implicar la extracción de datos de bases de datos, archivos, APIs, servicios web, etc.

Limpieza de datos: Los datos rara vez están limpios y listos para analizar. Es probable que necesites limpiarlos, lo que puede implicar tratar con datos faltantes, eliminar duplicados, corregir errores, etc.

Análisis Exploratorio de Datos (AED): Una vez que los datos están limpios, el siguiente paso es explorarlos para entender sus características principales. Esto puede implicar visualizar los datos, calcular estadísticas descriptivas, identificar outliers, examinar correlaciones entre variables, etc. El objetivo del AED es obtener una comprensión clara de los datos y formular hipótesis sobre posibles relaciones y patrones en los datos.

**Modelado de datos**: Después del AED, puedes comenzar a construir modelos de datos, como modelos de regresión, modelos de clasificación, clusters, etc., dependiendo del problema que estés tratando de resolver.

Evaluación del modelo: Una vez que tienes un modelo, necesitas evaluar su rendimiento. Esto puede implicar técnicas como la validación cruzada, el uso de conjuntos de prueba y validación, y el cálculo de métricas de rendimiento.

Interpretación y comunicación de resultados: Finalmente, interpretas los resultados de tu modelo y los comunicas a otras partes interesadas. Esto puede implicar la creación de visualizaciones, informes o presentaciones.


Source: https://nperci.org

<img src="https://www.questionpro.com/userimages/site_media/como-hacer-un-analisis-de-datos.jpeg" width="600" height="400">

---

## 1.3 Modelado de datos

La etapa de modelado utiliza la primera versión del conjunto de datos preparado y se enfoca en desarrollar modelos predictivos o descriptivos, a partir del uso de modelos estadísticos o matemáticos según el enfoque analítico previamente definido. La definición del modelo depende del objetivo con el que se vaya a realizar el AED, mediante la definición del objetivo podemos establecer el modelo (descriptivo y/o predictivo).

### 1.3.1 Tipos de Modelos

**Modelo Descriptivo**

El modelo descriptivo, se utiliza para describir o resumir un conjunto de datos o fenómenos observados. Su objetivo principal es comprender y comunicar las características, patrones o relaciones presentes en los datos y proporcionar información descriptiva sobre los datos. Se pueden platear preguntas como "¿qué está sucediendo?", "¿cuáles son las características principales de los datos?" o "¿cómo se relacionan las variables entre sí?". 

**Modelo Predictivo**

El modelo predictivo, se utiliza en un conjunto de capacitación (datos históricos en los que se conoce el resultado de interés) para construir el modelo, ya que su objetivo es predecir la probabilidad de éxito de un variable en función de variables específicas y hacer predicciones sobre eventos futuros. Este modelo busca responder preguntas como "¿qué sucederá en el futuro?", "¿cuál será el resultado de cierto evento?" o "¿cuál es la probabilidad de que ocurra un determinado resultado?".

Independientemente del modelo que se va utilizar, se debe hacer uso de herramientas o técnicas que ayuden a entender el tipo de modelo y el objetivo del análisis; en el modelo descriptivos se pueden utilizar técnicas como medidas de tendencia central (como la media o la mediana), medidas de dispersión (como la desviación estándar o el rango Inter cuartil) y en el modelo predictivo, se van a utilizar **_Algoritmos_ (regresión, clasificación o series de tiempo)**  que revisan los datos y que son capaces de predecir comportamientos futuros.

El proceso de modelado normalmente es muy iterativo, ya que las organizaciones están adquiriendo insights intermedios, lo que deriva en ajustes en la preparación de datos y en la especificación del modelo. Para una técnica determinada, se pueden probar múltiples algoritmos con sus respectivos parámetros para encontrar el mejor modelo para las variables disponibles. Cada método tiene ciertos puntos fuertes y es más adecuado para determinados tipos de problemas.

Para ambos tipos de modelos se va a necesitar gráficos y visualizaciones de datos, AED, técnicas de agrupamiento o clustering, análisis de componentes principales (PCA) y análisis de correlación, que van a buscar utilizar estos datos para hacer proyecciones, descripciones y/o toma de decisiones basadas en las predicciones.

<img src="https://data02.123doks.com/thumbv2/123dok_es/000/657/657991/37.894.179.743.117.398/figura-representaci%C3%B3n-general-modelos-tareas-miner%C3%ADa-datos.webp" width="600" height="400">



Source:  http://bigdatauniversity.com/bdu-wp/bdu-course/data-science-methodology


## 1.4 Métodos de Modelado

Los diferentes _Tipos de Modelo (descriptivo o predictivo)_ a implementar en áreas de la Inteligencia Artificial, tales como el Machine Learning, Ciencia de Datos o Big Data, permiten derivar nueva información procedente de los datos y desarrollar **Modelos predictivos**.

Para iniciar a Modelar datos en el Modelo Predictivo, existen algunos métodos de modelado que se dividen en estas categorías:

- No Supervisado.
  - Asociación.
  - Segmentación.
  
  
- Supervisado.

<img src="https://blogdatlas.files.wordpress.com/2020/06/datlas_ml_supervised_notsupervised.png" width="600" height="400">

    
## 1.4.1 Modelo No Supervisado

El **_Modelo No Supervisado_**, es un tipo de modelo de aprendizaje automático en el que no se proporciona una variable objetivo previamente. En cambio, el modelo busca patrones y estructuras inherentes en los datos sin etiquetas. El objetivo principal de un modelo no supervisado es encontrar agrupaciones, similitudes o relaciones ocultas en los datos. Este tipo de modelo exploran los datos sin ninguna guía específica y pueden revelar información valiosa sobre las características y estructuras subyacentes de los datos. Los modelos no supervisados se utilizan en diversos casos, como la segmentación de clientes, la detección de anomalías, la reducción de dimensionalidad y la recomendación de productos. Existen tipos de modelos No Supervisado como el **_Modelos de asociación y Modelos de segmentación_**.

**Modelos de asociación**

Los modelos de asociación encuentran patrones en los datos en los que una o más entidades (como eventos, compras o atributos) se asocian con una o más entidades. Los modelos construyen conjuntos de reglas que definen estas relaciones. Aquí los campos de los datos pueden funcionar como entradas y destinos. Podría encontrar estas asociaciones manualmente, pero los algoritmos de reglas de asociaciones lo hacen mucho más rápido, y pueden explorar patrones más complejos. Los modelos Apriori y Carma son ejemplos del uso de estos algoritmos. Otro tipo de modelo de asociación es el modelo de detección de secuencias, que encuentra patrones secuenciales en datos estructurados temporalmente.

Los modelos de asociación son los más útiles si se desean predecir varios resultados; por ejemplo, los clientes que adquirieron el producto X también adquirieron Y y Z. Los modelos de asociación relacionan una conclusión específica (como la decisión de adquirir un producto) con un conjunto de condiciones. La ventaja de los algoritmos de reglas de asociación sobre los algoritmos más estándar de árboles de decisión (C5.0 y Árbol C&R) es que las asociaciones pueden existir entre cualquiera de los atributos. Un algoritmo de árbol de decisión generará reglas con una única conclusión, mientras que los algoritmos de asociación tratan de buscar muchas reglas, cada una de las cuales puede tener una conclusión diferente.

**Modelos de segmentación**

Los modelos de segmentación dividen los datos en segmentos o clústeres de registros que tienen patrones similares de campos de entrada. Como sólo se interesan por los campos de entrada, los modelos de segmentación no contemplan el concepto de campos de salida o destino. 

Los modelos de segmentación (también conocidos como "modelos de agrupación en clústeres") son útiles en aquellos casos en los que se desconoce el resultado específico (por ejemplo, a la hora de detectar nuevos patrones de fraude o de identificar grupos de interés en la base de clientes). Los modelos de agrupación en clústeres se centran en la identificación de grupos de registros similares y en el etiquetado de registros según el grupo al que pertenecen. Esto se lleva a cabo sin la ventaja que ofrece el conocimiento previo sobre los grupos y sus características, y diferencia a los modelos de clústeres de otras técnicas de modelado en que no hay campos de salida u objetivo predefinidos para el modelo que se va a predecir. No hay respuestas correctas o incorrectas para estos modelos. Su valor viene determinado por su capacidad de capturar agrupaciones interesantes en los datos y proporcionar descripciones útiles de dichas agrupaciones. Los modelos de clúster se usan a menudo para crear clústeres o segmentos que se usan posteriormente como entradas en análisis posteriores, (por ejemplo, mediante la segmentación de clientes potenciales en subgrupos homogéneos).

## 1.4.2 Modelo Supervisado

Los Modelos supervisados utilizan los valores de uno o varios campos de entrada para predecir el valor de uno o varios resultados o campos de destino, algunos ejemplos de estas técnicas son: 

- Arboles de decisiones.
- **_Algoritmos de regresión._**
  - Lineal.
  - Logística.
  - Lineal generalizada.
  - Random forest.
- Redes neuronales.
- Máquinas de vectores de soporte.
- Redes bayesianas.

<img src="https://blogdatlas.files.wordpress.com/2020/06/datlas_regression-vs-classification-in-machine-learning.png" width="600" height="400">


Los modelos supervisados ayudan a las organizaciones a predecir un resultado conocido, por ejemplo, si un cliente comprará o se irá o si una transacción se ajusta a un patrón conocido de fraude. Las técnicas de modelado incluyen aprendizaje automático de las máquinas, inducción de reglas, identificación de subgrupos, métodos estadísticos y generación de varios modelos.

Ejemplos de casos de uso:

- Categorización de siniestros. Podría categorizar las zonas más siniestradas de una ciudad entrenando un modelo con la historia de datos. De esta manera se podría generar mejores rutas de patrullaje por los policías.

- Predecir el éxito. Para hoteles u hospedajes de AIRBNB podría predecir si van a tener éxito o no considerando las variables que comunican en sus anuncios.

**Algoritmos de Regresión**

Es útil para predecir productos continuos. La respuesta se presenta como cantidad. El valor predicho puede usarse para identificar la relación lineal entre atributos.

Ejemplos:

- Precios de vivienda. Estimar precios de inmuebles considerando variables como dimensión de propiedad, tamaño de construcción, pisos, recámaras y otras características.
- Predecir camas hospitalarias necesarias. Una oficina o secretaría de salud podría predecir con base a su histórico la cantidad de camas y doctores que serán necesarios el próximo año para atender a la demanda de la población. Un avance que pudiéramos llevar allá es con la cantidad de mujeres embarazadas.
- Identificar las cervezas que necesitarás en tu inventario. Predecir la cantidad de inventarios es una de las aplicaciones más usadas en el sector retail.

**Técnicas**

**Regresión lineal:**
La regresión lineal es un método de modelado estadístico que se utiliza para predecir o estimar el valor de una variable dependiente continua en función de una o más variables independientes. El objetivo es encontrar la mejor línea recta que se ajuste a los datos y minimice la diferencia entre los valores observados y los valores predichos. Se asume una relación lineal entre las variables y se utilizan técnicas como el método de los mínimos cuadrados para calcular los coeficientes de la línea recta. La regresión lineal es ampliamente utilizada en diversos campos para realizar predicciones y analizar relaciones entre variables.

**Regresión no lineal:**
La regresión no lineal es similar a la regresión lineal, pero permite modelar relaciones no lineales entre las variables dependientes e independientes. En lugar de ajustarse a una línea recta, los modelos de regresión no lineal se ajustan a curvas más complejas, como polinomios, exponenciales, logaritmos, entre otros. Estos modelos pueden capturar relaciones más flexibles y pueden ser más adecuados cuando los datos muestran patrones no lineales. La regresión no lineal se utiliza en diversas áreas, como ciencias de la salud, economía, física, entre otras, para modelar y predecir fenómenos más complejos.

**Regresión Logística:**
La regresión logística es un algoritmo de aprendizaje supervisado que se utiliza para predecir la probabilidad de pertenencia a una clase específica en función de variables predictoras. En este caso, el modelo se entrena con datos de juegos existentes (género y plataforma) y su éxito o no éxito en términos de ventas globales. Luego, se utiliza para predecir si una nueva idea de juego será exitosa o no, en función de su género y plataforma.

**Máquinas de soporte de vectores (support vector machines):**
Las máquinas de vectores de soporte son un algoritmo de aprendizaje supervisado utilizado tanto para clasificación como para regresión. El objetivo principal de las SVM es encontrar el hiperplano óptimo que maximiza el margen entre las clases en un espacio dimensional más alto. Utiliza puntos de datos de entrenamiento llamados vectores de soporte para definir el hiperplano y clasificar nuevas instancias en una de las dos clases. Las SVM son conocidas por su capacidad para manejar conjuntos de datos complejos y de alta dimensión, y han demostrado ser efectivas en aplicaciones como reconocimiento de imágenes, clasificación de texto y detección de anomalías.

**Redes Neuronales Artificiales:**
Las redes neuronales son modelos de aprendizaje automático inspirados en el funcionamiento del cerebro humano. Están compuestas por múltiples capas de neuronas artificiales interconectadas, donde cada neurona realiza cálculos y transmite señales a través de conexiones ponderadas. Estas redes pueden aprender y adaptarse a partir de datos para realizar tareas de clasificación, regresión o reconocimiento de patrones. Cada capa de neuronas procesa y extrae características de los datos de entrada, lo que permite un aprendizaje profundo y la detección de relaciones complejas. Las redes neuronales se utilizan en una amplia gama de aplicaciones, como reconocimiento de imágenes, procesamiento del lenguaje natural, análisis de datos y más.

**Aprendizaje profundo (deep learning):**
El aprendizaje profundo es una rama del aprendizaje automático que se basa en redes neuronales profundas. Utiliza algoritmos de aprendizaje automático para entrenar redes neuronales con múltiples capas ocultas, lo que permite un aprendizaje jerárquico de características complejas en los datos. El aprendizaje profundo se caracteriza por su capacidad para extraer y aprender representaciones de alto nivel de los datos de entrada, lo que puede conducir a un rendimiento mejorado en tareas de reconocimiento, clasificación, generación de contenido y toma de decisiones. Es especialmente efectivo cuando se trabaja con grandes conjuntos de datos y problemas complejos. El aprendizaje profundo ha impulsado avances significativos en áreas como el procesamiento de imágenes y el procesamiento del lenguaje natural.

**Bosques aleatorios (random forests):**
Los bosques aleatorios son un conjunto de árboles de decisión que trabajan juntos para realizar clasificación o regresión. Cada árbol se entrena en una muestra aleatoria de datos y realiza una votación para determinar la clasificación final o el valor de regresión. Los bosques aleatorios tienen la capacidad de manejar grandes conjuntos de datos con alta dimensionalidad.


Source: https://www.ibm.com/docs/es/spss-modeler/saas?topic=mining-types-models

---

# 2. Objetivo del Proyecto

Realizar un AED en base a la Hipótesis del tema de Tesis y obtener información valiosa que permita la toma de decisiones para establecer el tipo de 'Genero' y/o 'Plataforma' del Serious Games a desarrollar.

## 2.1 Desarrollo del Objetivo

En base al **_Objetivo de Proyecto_** se plantea realizar un **AED** y un **Modelo de Datos** para establecer uno de los Objetivos del Tema de Tesis.


## 2.2 Descripción del Objetivo en base al Tema de Tesis:

Diseñar un _**Serious Game**_ para el aprendizaje de cinemática utilizando la metodología de Aprendizaje Basado en Problemas (ABP).

---

# 4. Metodología de Desarrollo

Para realizar un **AED** y **Modelo de Datos** que pueda permitir **establecer el tipo de Genero y/o Plataforma del Serious Games a desarrollar**, se va trabajar cada tarea de la siguiente forma:

1. Definición de la(s) _Variable(s) Objetivo(s)._

2. Data Clean:
   - Carga de Datos
   - Preprocesar los datos.
   - Eliminar variables irrelevantes.
   - imputar valores faltantes.
   - Limpiar los nombres de los atributos que no se vayan a utilizar.

3. Realizar un AED de los datos para entender la distribución de las variable(s) objetivo(s) y las variables para conseguir el objetivo del proyecto:

   - Análisis de Correlación de Ventas Globales por Consola y Genero.
   - Análisis de Ventas Globales de Videojuegos por Plataforma.
   - Análisis de Ventas Globales por Género.
   - Análisis de Ventas Globales por Compañía de Desarrollo.

4. Generar un Modelo Predictivo Supervisado con Algoritmo de:

   - Regresión: Este algoritmo puede predecir un valor continuo (como las ventas globales de un videojuego). Se trata de encontrar una relación entre las variables de entrada y la variable de salida que puede ser representada como una ecuación matemática. Los algoritmos de regresión son: regresión lineal, la regresión polinomial y la regresión de árbol de decisión.

   - Clasificación: Este algoritmo puede predecir una categoría o clase (como el género de un videojuego). Se trata de encontrar una frontera de decisión que separe las diferentes clases en el espacio de las variables de entrada. Los algoritmos de clasificación son: regresión logística, los árboles de decisión, las máquinas de vectores de soporte y las redes neuronales.

   - Predicción: Este algoritmo se utiliza para predecir. La diferencia radica en el tipo de variable de salida que se trata de predecir.

5. Evaluar el modelo.

6. Implementar el modelo.

7. Retroalimentación del modelo.
---


## 4.1 Definición de la(s) Variable(s) Objetivo(s).

**El objetivo es clasificar el 'Genero de juego' y la 'Plataforma'**, ya sea de forma separada o conjunta, para obtener la información de que tipo de Genero y Plataforma se puede desarrollar el Serious Games; por lo tanto, la correlación, clasificación y predicción del Género y Plataforma de Juego estará dada **por el análisis de Videojuegos Exitosos**.

La **variable objetivo** será determinar qué tipo de género de juego y plataforma serán útiles para la creación de un nuevo videojuego exitoso. En este contexto, **el éxito de un Videojuego** esta dado **por la cantidad de Copias Vendidas del Videojuego que está definido en el atributo 'Ventas Globales'**, por lo que las **Variables** a utilizar para alcanzar el **Objetivo** del proyecto pueden incluir:

**Género del juego:** Esta variable representa la categoría o tipo de juego al que pertenece, como acción, aventura, estrategia, deportes, etc.

**Plataforma:** Esta variable indica el sistema o dispositivo en el que el juego será lanzado y jugado, como PlayStation, Xbox, PC, Nintendo Switch, etc.

**Ventas Globales:** Esta variable representa las ventas totales del juego en todo el mundo. Se va a **utilizar** como una **medida de éxito** para determinar **si un juego es exitoso o no**.

Otras variables: También se pueden considerar otras variables relevantes para el análisis, como el rating del juego, las puntuaciones de reseñas, la compañía de desarrollo, la fecha de lanzamiento, etc., dependiendo de la disponibilidad de datos y la relevancia para el objetivo específico.

---

# 5. Data Clean

## 5.1 Descripción de los datos

En este proyecto se cuenta con un conjunto de datos obtenidos a través de Web Scraping de las paginas web:
- https://www.mobygames.com
- https://www.kaggle.com/datasets/sidtwr/videogames-sales-dataset
- https://www.kaggle.com/datasets/gregorut/videogamesales

Los data sets están en formato CSV y son:
- consolas.csv
- consolas2.csv
- juegos_mas_vendidos.csv
- vgsales.csv
- video_games.csv

La información que contiene los archivos CSV es la siguiente:

**consolas.csv & consolas2.csv** : Contiene información de las plataformas de videojuego, juegos desarrollados, y críticas.

   - Atributos: 
   
     - Platform: Este atributo es de tipo string y describe el nombre de la consola de juegos para la cual se desarrollaron los juegos.

     - Games_x: Este atributo es de tipo entero y representa la cantidad de juegos que se han desarrollado para la consola específica representada en la columna "Platform".
    
     - Player Reviews: Este atributo es de tipo entero y muestra la cantidad de comentarios o críticas realizadas por los jugadores acerca de la consola.

     - Critic Reviews: Este atributo es de tipo entero y muestra la cantidad de críticas realizadas por críticos profesionales acerca de la consola.

     - Companies: Este atributo también es una combinación de cadena de texto e integer y muestra la cantidad de compañías de desarrollo de videojuegos que han desarrollado títulos para la consola.

     - Years: Este atributo es una cadena de texto con datos enteros que indica el rango de años durante los cuales la consola ha estado en el mercado. Por ejemplo, un valor de "2001 - 2020" indicaría que la consola se lanzó en 2001 y se sigue utilizando hasta 2020.

**juegos_mas_vendidos.csv & vgsales.csv & video_games.csv**: Contiene información de los juegos mas vendidos por plataforma, genero, etc., y estadisticas del promedio de tiemp que pasa el jugador jugando.

- Atributos: 

    - 'Titulo': tipo string El nombre del videojuego.

    - 'Compañia de desarrollo': tipo string La empresa o estudio que desarrolló el videojuego.

    - 'Fecha de Lanzamiento': tipo int La fecha en que el videojuego fue lanzado oficialmente al mercado.

    - 'Genero': tipo string El tipo o categoría de juego al que pertenece el videojuego (ej. acción, aventura, estrategia, etc.).

    - 'Plataforma': tipo string El sistema o dispositivo en el que el juego fue lanzado y puede ser jugado (ej. PlayStation, Xbox, PC, etc.).

    - 'Multiplataforma': tipo string Un indicador de si el videojuego está disponible en más de una plataforma.

    - 'Portatil': tipo bool Un indicador de si el videojuego está disponible en plataformas portátiles (ej. Nintendo Switch, PSP, etc.).

    - 'Online': tipo bool Un indicador de si el videojuego tiene funcionalidad de juego en línea.

    - 'Max Jugadores': tipo bool El número máximo de jugadores que pueden jugar el videojuego simultáneamente.

    - 'Rating': tipo int La clasificación de edad o recomendación de edad para el videojuego (ej. E para todos, T para adolescentes, M para maduro, etc.).

    - 'Ranking': tipo int El lugar que ocupa el videojuego en una lista ordenada, generalmente en términos de popularidad o ventas.

    - 'Puntuacion Reseña': tipo float La calificación o puntuación promedio que los críticos de videojuegos han dado al videojuego.

    - 'Secuela': tipo bool Un indicador de si el videojuego es una secuela de un videojuego anterior.

    - 'Licenciado': tipo bool Un indicador de si el videojuego está basado en una licencia existente (ej. una película, una serie de televisión, un cómic, etc.).

    - 'Ventas NA': tipo float La cantidad de copias del videojuego que se han vendido en América del Norte.

    - 'Ventas EU': tipo float La cantidad de copias del videojuego que se han vendido en Europa.

    - 'Ventas JP': tipo float La cantidad de copias del videojuego que se han vendido en Japón.

    - 'Ventas Otros': tipo float La cantidad de copias del videojuego que se han vendido en otras regiones del mundo.

    - 'Ventas Globales': tipo float La cantidad total de copias del videojuego que se han vendido en todo el mundo.

    - 'Ventas Estimadas': tipo float Una estimación de la cantidad total de copias del videojuego que se venderán en el futuro, basada en las tendencias actuales de ventas.

    - 'Length.All PlayStyles.Average':  tipo float Representa la duración promedio de juego teniendo en cuenta todos los estilos de juego.

    - 'Length.All PlayStyles.Leisure':  tipo float Muestra la duración de juego para aquellos jugadores que disfrutan el juego de una manera más relajada o casual, abarcando todos los estilos de juego.

    - 'Length.All PlayStyles.Median':  tipo float Es la mediana de la duración de juego, tomando en cuenta todos los estilos de juego.

    - 'Length.All PlayStyles.Polled':  tipo float Número de observaciones o muestras utilizadas para calcular la duración promedio de todos los estilos de juego.

    - 'Length.All PlayStyles.Rushed':  tipo float Refleja la duración de juego para aquellos jugadores que avanzan de manera más apresurada, considerando todos los estilos de juego.

    - 'Length.Completionists.Average':  tipo float Es la duración promedio de juego para aquellos jugadores completistas, quienes se esfuerzan por alcanzar el 100% del juego.

    - 'Length.Completionists.Leisure':  tipo float Muestra la duración del juego para los jugadores completistas que juegan de manera más relajada o casual.

    - 'Length.Completionists.Median':  tipo float Es la mediana de la duración de juego para los jugadores completistas.

    - 'Length.Completionists.Polled':  tipo float Número de observaciones o muestras utilizadas para calcular la duración promedio de los jugadores completistas.

    - 'Length.Completionists.Rushed':  tipo float Representa la duración de juego para los jugadores completistas que avanzan a través del juego de una manera más apresurada.

    - 'Length.Main + Extras.Average':  tipo float Muestra la duración promedio de juego cuando se juega la historia principal además de los contenidos extras.

    - 'Length.Main + Extras.Leisure':  tipo float Duración del juego para aquellos jugadores que disfrutan la historia principal y los contenidos extras de una manera más relajada o casual.

    - 'Length.Main + Extras.Median':  tipo float Es la mediana de la duración del juego, considerando la historia principal y los contenidos extras.

    - 'Length.Main + Extras.Polled':  tipo float Número de observaciones o muestras utilizadas para calcular la duración promedio del juego principal más los contenidos extras.

    - 'Length.Main + Extras.Rushed':  tipo float Refleja la duración de juego para aquellos jugadores que avanzan de manera más apresurada a través de la historia principal y los contenidos extras.

    - 'Length.Main Story.Average':  tipo float Muestra la duración promedio de la historia principal del juego.

    - 'Length.Main Story.Leisure':  tipo float Representa la duración de la historia principal del juego para aquellos jugadores que la disfrutan de una manera más relajada o casual.

    - 'Length.Main Story.Median':  tipo float Es la mediana de la duración de la historia principal del juego.

    - 'Length.Main Story.Polled':  tipo float Número de observaciones o muestras utilizadas para calcular la duración promedio de la historia principal.

    - 'Length.Main Story.Rushed':  tipo float Indica la duración de la historia principal del juego para aquellos jugadores que la avanzan de manera más apresurada.

</small>

Diagrama Entidad Relacion
<img src="img/Proyecto_Final.png" width="600" height="400">

---


## 5.3 Preprocesar los datos
###  Fusionar data frames

Se van a fusionar dos DataFrames (df_consolas y df_consolas2), los atributos en común son "Platform" que representa el nombre de la Plataforma en que se ejecuta el Videojuego.

Se van a fusionar tres DataFrames (df_juegos, df_vgsales, df_video_games), los atributos en común son "Título" en df_juegos, "Name" en df_vgsales y "Title" en df_video_games que representa el nombre del videojuego.

### Eliminar variables irrelevantes


El DataFrame df_consolas, se va eliminar el atributo 'Games_y' ya que se repite con el atributo 'Games_x', y se van a renombrar los atributos resultantes:
- 'Platform': 'Plataforma',
- 'Companies': 'Compañia',
- 'Games_x': 'Juegos_Desarrollados',
- 'Years': 'Anios',
- 'Player Reviews': 'Resenas_Jugador',
- 'Critic Reviews': 'Cantidad_Criticas'  

Se van a remplazar todos los valores nulos (NaN) en el DataFrame de acuerdo con el tipo de dato como lo son:
- 'Plataforma' con 'Desconocido'.
- 'Compañia' con 'Desconocido'.
- 'Juegos_Desarrollados con 0.
- 'Anios' con 0.
- 'Resenas_Jugador' con 0.
- 'Cantidad_Criticas' con 0.

Del DataFrame df_juegos se realiza un procesado mas amplio de los datos:

- Se va reemplazar los valores nulos en la columna 'Genre_x' con los valores correspondientes de la columna 'Genre_y'.

- Se  va eliminar la columna 'Genre_y' del DataFrame, esto se hace porque ya se lleno los valores nulos en 'Genre_x' con los valores correspondientes.

- Se van a eliminar las columnas: 'Fecha_Lanzamiento', 'Unnamed: 11', 'Fecha_Lanzamineto', 'Desarrollador_y', 'Genre', 'Desarrollador_x' y 'Distribuidor'.

- Se van a renombrar las columnas del DataFrame y se proporciona un diccionario en el que se especifica el nuevo nombre de cada columna.

- Se reorganizan las columnas para una mejor comprensión.

- Se define una lista llamada 'columnas' que contiene los nombres de las columnas que se van a modificar, y se va iterar sobre cada columna en la lista para reemplazar los valores nulos que tengan.

- Para los atributos de tipo string se va remplazar los espacios vacios con por 'Desconocido'.
  
- Se define una lista llamada 'valores_incorrectos' ('2007', '2009', '2010', '2011', '2012', '2013', '2014', '2015'), que contiene los valores que se van a reemplazar en el atributo Genero por 'Desconocido'.

- Para los atributos de tipo int o float se va remplazar los espacios vacios con 0.
- Para los atributos de tipo bool se van a remplazar los espacios vacios con 'False'.

## 6 Análisis exploratorio de Datos (AED)

En el análisis exploratorio se analizan los DataFrames con la información proporcionada en la sección anterior, el propósito es analizar e investigar los conjuntos de datos, resumir sus características principales, identificar relaciones, entender la distribución de la(s) variables(s) objetivo(s) y las variables para conseguir el objetivo del proyecto.

Se define a realizar lo siguiente:

- #### Análisis de Ventas Globales por año.
- #### Análisis de Correlación de Ventas Globales por Consola y Genero.
- #### Análisis de Ventas Globales de Videojuegos por Plataforma.
- #### Análisis de Ventas Globales por Género.
- #### Análisis de Ventas Globales por Compañía de Desarrollo.
---

## 6.1 Análisis de Ventas Globales por año.

En este análisis, se examina la distribución de las ventas de videojuegos a nivel global a lo largo de los años utilizando el atributo 'Fecha_Lanzamiento' que contiene la información de la fecha en que se lanzó a la venta del videojuego y el atributo 'Ventas_Globales' que contiene la información del total de ventas globales del videojuego, por lo que la relación de las ventas globales con el año de lanzamiento se visualiza en un gráfico lineal.
El objetivo es identificar patrones o tendencias en las ventas a lo largo del tiempo, como picos o declives en ciertos años. Esto puede ayudar a comprender la evolución de la industria de los videojuegos y tomar decisiones estratégicas basadas en las ventas históricas.

---

### 6.1.1 información relevante:

- El promedio de ventas globales tiene un promedio de 500000 mil copias en el lapso de 37 años.
- Los picos más altos de ventas Globales están entre 2007 y 2008.
- La tendencia de ventas incremento a partir del año 2000, pero a partir de 2015 las ventas bajaron.

---


## 6.2 Análisis de Correlación de Ventas Globales por Consola y Genero.

Se puede explorar las correlaciones entre los diferentes atributos que se tienen en el DataFrame df_juegos para ayudar a entender mejor sus relaciones y seleccionar las características para el modelado de datos.

La matriz de correlación es una tabla que muestra el coeficiente de correlación (también conocido como Pearson's r) entre pares de variables en un conjunto de datos. Cada celda de la tabla muestra la correlación entre dos variables.

Las características de la matriz de correlación son:

- Coeficiente de correlación que es una medida estadística que describe el grado de relación entre dos variables.
- El coeficiente de correlación puede variar de -1 a +1.
- Una correlación de +1 indica una fuerte correlación positiva: esto significa que las dos variables tienden a aumentar juntas.
- Una correlación de -1 indica una fuerte correlación negativa: esto significa que a medida que una variable aumenta, la otra disminuye.
- Una correlación de 0 indica que no hay una relación lineal entre las variables.

---

Al visualizar la matriz de correlación con el mapa de calor, se puede obtener una vista de cómo están correlacionadas las variables en el conjunto de datos del DataFrame df_juegos.

En el mapa de calor:

- Las celdas coloreadas representan las correlaciones entre las variables.
- El color de cada celda se determina según el valor de correlación y el mapa de color que se utiliza.
- Las correlaciones fuertes (cercanas a 1 o -1) se indican con colores más intensos, mientras que las correlaciones débiles (cercanas a 0) se indican con colores más claros.

**Se visualiza una fuerte correlación positiva entre las 'Ventas_Globales', 'Ranking' y la 'Puntuacion_Reseña', por lo que se puede inferir que los videojuegos con puntuaciones de reseñas más altas tienden a tener más ventas globales. Esto sugiere que la calidad de un juego (según lo medido por las reseñas) puede influir en su éxito comercial. Sin embargo, la correlación no implica causalidad y se va necesita más investigación para entender la relación entre estas variables.**

---

### 6.2.1 Relación entre Genero y Ventas Globales**

Para profundizar en el análisis de correlación, se va a graficar las relaciones entre tres variables: 'Plataforma', 'Ventas_Globales', y 'Genero'. La variable 'Plataforma' se muestra a lo largo del eje x, la variable 'Ventas_
Globales' se muestra a lo largo del eje y, y la variable 'Genero' se representa mediante el color de los puntos.

Por lo tanto, cada punto en el gráfico representa un juego, y su posición en el eje x y y indica la plataforma en la que se lanzó el juego y las ventas Globales que tuvo. El color del punto indica el género del juego.

Se observa en cada punto del gráfico cómo las ventas en Globales varían según la plataforma y el género.

---

Los puntos de un color específico (videojuegos de un cierto género) están concentrados en una cierta área del gráfico, sugiere que el género tiende a tener más ventas en determinadas plataformas.

### 6.2.2 información relevante:
- **El promedio de ventas globales de cada genero están por debajo de las 10 millones de copias, por lo tanto, es de sugerir hacer una análisis de los promedios de ventas globales por genero y/o plataforma.**
- Los géneros que más venden son el de Accion, Racing, Platform, Role Playing y Shooter.
- Las plataformas que más venden por genero son:
  - Accion (Nintendo, Play Station y Xbox).
  - Racing (Nintendo, Play Station y Xbox).
  - Accion (Nintendo, Play Station y Xbox).
  - RPG (Nintendo, Play Station y Xbox).
  - Shooter (Play Station y Xbox).
  
  ---
  
  
  ## 6.3 Análisis de Ventas Globales de Videojuegos por Plataforma.

Resultado del análisis de correlación anterior, se puede observar que la relación entre las 'Ventas_Globales', 'Genero' y 'Plataforma' está por debajo de 1 millón de copias, por lo tanto, se va realizar una análisis de la media de 'Ventas_Globales.

En este análisis, se examina la distribución de las ventas de videojuegos según la plataforma en la que se juegan, utilizando el atributo 'Plataforma' que contiene la información de la plataforma en la que se ejecuta el videojuego y el atributo 'Ventas_Globales' que contiene la información del total de ventas globales del videojuego, por lo que la relación puede calcular el total de ventas por Plataforma y visualizar esta información en un gráfico lineal marcando cada punto máximo en el atributo 'Plataforma' de los videojuegos más populares o exitosos en términos de ventas. Esto puede ser útil para comprender el mercado de consolas y tomar decisiones sobre el desarrollo y la distribución de juegos específicos para ciertas plataformas.

---

### 6.3.1 información relevante:
- El promedio de ventas globales por plataforma están por debajo de 1 millón de copias.
- El promedio total de ventas globales para todas las plataformas es de 548394 millones de copias.
- Las plataformas que más venden son de Nintendo, Play Station y Xbox.


## 6.4 Análisis de Ventas Globales por Género.
En este análisis, se examina la distribución de las ventas de videojuegos a nivel global utilizando el atributo 'Genero' que contiene la información del género del videojuego y el atributo 'Ventas_Globales' que contiene la información del total de ventas globales del videojuego, por lo que la relación puede calcular el total de ventas por género y visualizar esta información en un gráfico lineal marcando cada punto máximo en el atributo 'Genero' de videojuegos más populares o exitosos en términos de ventas. Esto puede ser útil para tomar decisiones relacionadas con el desarrollo y la comercialización de nuevos juegos, así como para comprender los intereses y preferencias de los jugadores.

---

### 6.4.1 información relevante:

- El promedio de ventas globales por genero están por debajo de 1 millones de copias.
- El promedio total de ventas globales para todos los Géneros es de 548394 millones de copias.
- Los Géneros que más venden son:
  - Arcade.
  - SandBox.
  - Platform.
  - Shooter.
  - RPG.
  - Racing.
  - Sports.
  - Accion.
  
  ---
  
  ## 6.5 Análisis de Ventas Globales por Compañía de Desarrollo.

En este análisis, se examina la distribución de las ventas de videojuegos a nivel global según la compañía de desarrollo de los juegos, utilizando el atributo 'Compañia_Desarrollo' que contiene la información de la compañía que desarrollo el videojuego y el atributo 'Ventas_Globales' que contiene la información del total de ventas globales del videojuego, por lo que la relación puede calcular el total de ventas por compañía y visualizar esta información en un gráfico de lineal.
El objetivo es identificar qué compañías de desarrollo tienen mayor éxito en términos de ventas de videojuegos. Esto puede ser útil para evaluar la reputación y el rendimiento de las compañías de desarrollo y tomar decisiones sobre asociaciones o adquisiciones en la industria.

---


### 6.5.1 información relevante:

La mayoría de las Compañías de Desarrollo tienen un promedio de ventas Globales debajo de 500000 mil copias.
Las Compañías de Desarrollo que más venden son:
- Nintendo.
- Electroni Arts.
- Activision.
- Sony.
- Ubisoft.

---

# 7. Resultados de AED

Para relacionar los análisis al modelado de datos, se resume los puntos fuertes del tipo de análisis acorde con el objetivo del proyecto:



- **Análisis de Correlación de Ventas Globales por Consola y Genero:**

  - Se puede examinar la correlación entre los atributos del DataFrame df_juegos.
  - Se puede identificar la correlación positiva entre las 'Ventas_Globales', 'Ranking' y la 'Puntuacion_Reseña'.
  - Se puede evaluar qué que los videojuegos con puntuaciones de reseñas más altas tienden a tener más ventas globales y que se puede usar como variable objetivo para definir el Serious Games, considerando las reseñas y el ranking que el jugador puede tener al jugar un videojuego, y como este puede desarrollar una experiencia de juego enfocada a la experiencia educativa.
  - En conclusión, se pueden utilizar estos datos para determinar en qué género del videojuego se debe desarrollar el Serious Games.
  
  
  
- **Análisis de Ventas Globales de Videojuegos por Plataforma:**

  - Se puede examinar la distribución de las ventas de videojuegos según la plataforma o consola en la que se juegan.
  - Se puede identificar qué plataformas son más populares en términos de ventas.
  - Se puede evaluar qué plataformas son más adecuadas para el Serious Games, considerando las características técnicas y de usabilidad requeridas para ofrecer una experiencia educativa efectiva.
  - En conclusión, se pueden utilizar estos datos para determinar en qué plataformas se debe desarrollar y distribuir el Serious Games.
  
  
  

- **Análisis de Ventas Globales por Género:**
  - Se puede examinar la distribución de las ventas de videojuegos según el género.
  - Se puede identificar los géneros de videojuegos más populares en términos de ventas.
  - Se puede evaluar qué géneros son relevantes para el Serious Games, considerando el objetivo educativo o informativo del juego.
  - En conclusión, se pueden utilizar estos datos para determinar qué género de Serious Games tiene un mayor potencial de aceptación y éxito en el mercado.
  
  
  

- **Análisis de Ventas Globales por Compañía de Desarrollo:**

  - Se puede examinar la distribución de las ventas de videojuegos según la compañía de desarrollo.
  - Se puede identificar qué compañías tienen un historial exitoso en términos de ventas de videojuegos.
  - Se puede evaluar posibles asociaciones o colaboraciones con estas compañías para el desarrollo y distribución del Serious Games.
  - En conclusión, se pueden utilizar estos datos para seleccionar una compañía de desarrollo con experiencia en el género de juegos y plataforma seleccionados.




Al combinar estos análisis, se puede obtener una visión más completa y respaldada por datos del tipo de género y plataforma más adecuados para el desarrollo del Serious Games. Estos análisis proporcionarán información sobre las preferencias de los jugadores, las tendencias del mercado y las oportunidades para lograr el éxito en términos de ventas y aceptación del juego. Y permitir crear un modelo predictivo para saber en base al 'Genero', 'Plataforma' y 'Ventas_Globales' **"si el desarrollo de un Serious Game puede ser exitoso"**.

---

# 8. Modelado de Datos


El modelado de datos se refiere al proceso de construcción de algoritmos (Machine Learning, Data Scinece, Big Data, entre otros), que pueden realizar predicciones o estimaciones sobre resultados futuros. En el contexto del **_Objetivo del proyecto_**, el modelado de datos que se va a desarrollar es para predecir el éxito o aceptación de un determinado género de juego en una plataforma específica.

Para aplicar el modelado de datos predictivo a esta hipótesis, se realizan los siguientes pasos:

- Recopilación de datos: Obtener un conjunto de datos históricos que contenga información relevante sobre juegos similares al Serious Games que se desea desarrollar. Estos datos deben incluir características del juego, como género, plataforma, ventas, reseñas, etc.

- Preparación de datos: Limpiar y preprocesar los datos, eliminando valores atípicos, datos faltantes y realizando transformaciones necesarias.

- Selección de variables: Identificar las variables o características del juego que pueden influir en su éxito o aceptación. Esto puede incluir el género, plataforma, características específicas del juego, datos demográficos de los jugadores, etc.

- Construcción del modelo: Seleccionar el algoritmo de aprendizaje automático adecuado para el tipo de problema y datos disponibles. Algunos ejemplos podrían ser regresión logística, árboles de decisión, bosques aleatorios o redes neuronales.

- Entrenamiento del modelo: Utilizar los datos históricos para entrenar el modelo, ajustando los parámetros del algoritmo y optimizando su rendimiento.

- Validación del modelo: Evaluar el rendimiento del modelo utilizando técnicas como la validación cruzada o la división de datos en conjuntos de entrenamiento y prueba. Medir métricas de rendimiento como precisión, recall, puntaje F1, etc.

- Predicción y toma de decisiones: Utilizar el modelo entrenado para realizar predicciones sobre el éxito o aceptación de un determinado género de juego en una plataforma específica. Estas predicciones pueden ayudar en la toma de decisiones sobre el tipo de género y plataforma a desarrollar para el Serious Games.

---

## 8.1 Recopilación de datos

Son los datos recopilados en formato csv y llamados:
- consolas.csv.
- consolas2.csv.
- juegos_mas_vendidos.csv.
- vgsales.csv.
- video_games.csv.



## 8.2 Preparación de datos


Se tiene dos Data Frames resultantes:
- df_consolas.
- df_juegos.

A partir del AED se concluyó que solo se va a utilizar df_juegos, por contener la información más cercana al objetivo del proyecto.



## 8.3 Selección de variables


Las variables para utilizar y crear el modelo son:
- 'Género'.
- 'Plataforma'.
- 'Ventas_Globales'.

Y su correlación positiva con:
- 'Ranking'.
- 'Puntuacion_Reseña'.

---

## 8.4 Construcción del modelo

En base al análisis de los diferentes resultados del AED, se tomó la decisión de crear varios "Modelos de Datos", por la razón de tener un porcentaje mayor de éxito al Objetivo del proyecto. Los modelos por crear son Modelos Supervisados, porque van a utilizar un conjunto de datos etiquetados, donde se conocen las 'Ventas_Globales' de los videojuegos (variable objetivo).

Los modelos por implementar:

- Modelo de Clasificación: para predecir la categoría género de un videojuego con las variables de entrada que va a usar el algoritmo de clasificación **_Random Forest_**.

- Regresión lineal, que se va a usar para entrenar el modelo y ajustar los coeficientes de la regresión. La selección de este algoritmo es porque puede encontrar la mejor línea recta que se ajuste a los datos para predecir la variable objetivo. El modelo de regresión lineal va a predecir las ventas globales de videojuegos en función de las variables utilizadas ('Género', 'Plataforma' y 'Compañía de desarrollo'). Estas variables tienen características para predecir las ventas globales de los videojuegos y encontrar posibles relaciones o patrones entre ellas y las ventas globales.


---

## 8.4.1 Modelo de Clasificación

El modelo se define en los siguientes pasos:


- Predecir la categoría 'Genero'.
- Implementar el algoritmo Random Forest: es un algoritmo potente y versátil que puede manejar tanto variables categóricas como numéricas.
- El algoritmo va a encontrar una frontera de decisión que separe las diferentes clases en el espacio de las variables de entrada.
- Las variables de entrada son 'Plataforma', 'Ranking', 'Puntuacion_Reseña' y 'Ventas_Globales'.
- La variable 'Plataforma' es categórica, por lo que se va a codificar usando el proceso llamado codificación one-hot. 
- Dividir los datos en conjuntos de entrenamiento y prueba.
- Predecir las etiquetas para los datos de prueba.
- Calcular la precisión del modelo.
- Mostrar el informe de clasificación.

---


## 8.4.2 Resultados del Modelo de Clasificación

Los resultados en base al informe de clasificación:


- La precisión del modelo (Accuracy) es aproximadamente 0.23 o 23%, lo que significa que el modelo predice correctamente el género del videojuego en un 23% de los casos en el conjunto de pruebas. En términos generales, esto no es muy bueno.

- La matriz de confusión muestra cuántas veces se predijo correcta o incorrectamente cada clase. Por ejemplo, la primera fila corresponde a la clase "Action". De 766 juegos de acción reales, el modelo predijo correctamente 275 de ellos. Sin embargo, también predijo incorrectamente 48 como "Adventure", 35 como "Fighting", 67 como "Misc", etc.



El informe de clasificación proporciona más detalles sobre el rendimiento del modelo para cada clase de acuerdo con las métricas:



- Precisión (Precisión): Es la proporción de predicciones positivas que fueron correctas, cuando el modelo predice "Action", es correcto el 35% de las veces.


- Recall: Es la proporción de casos positivos reales que fueron detectados correctamente, el modelo detecta 36% de los juegos de acción reales.


- F1-score: Es una métrica que combina precisión y recall en una sola cifra. Es útil cuando se quiere comparar dos o más modelos, especialmente si no tienes una preferencia específica entre precisión y recall.

- Soporte (Support): Es el número de ocurrencias de cada clase en el conjunto de pruebas.


Estos resultados sugieren que el modelo tiene problemas para predecir el género de los videojuegos basándose en las variables de entrada que se han utilizado. Puede ser útil explorar otras variables, crear nuevas características, usar otro algoritmo de clasificación o ajustar los parámetros del modelo actual para tratar de mejorar el rendimiento.


---

## 8.4.3 Modelo de Regresión

El modelo se define en los siguientes pasos:

- Predecir la característica 'Ventas_Globales’.
- Implementar el algoritmo regresión lineal: es un enfoque estadístico para modelar la relación entre una variable dependiente (o variable objetivo) y una o más variables independientes (o características).
- El algoritmo va a predecir las 'Ventas_Globales' basándose en las características 'Genero', 'Plataforma' y 'Compañia_Desarrollo'.
- Las variables de entrada son 'Genero', 'Plataforma' y 'Compañia_Desarrollo'.
- Definir de las características y el objetivo: 'Genero', 'Plataforma' y 'Compañia_Desarrollo' son características, y 'Ventas_Globales' es el objetivo.
- Convertir las características categóricas a numéricas, se va a utilizar variables ficticias (o dummies) para convertir estas características categóricas en numéricas.
- Dividir los datos en conjuntos de entrenamiento y prueba.
- Crear y entrenar el modelo de regresión lineal.
- Predecir las ventas globales para el conjunto de prueba
- Resultados del modelo de predicción.


---

## 8.4.4 Entrenamiento del modelo

El modelo se entrena utilizando las características 'Genero', 'Plataforma' y 'Compañia_Desarrollo' para predecir las ventas globales de los videojuegos. Las características categóricas se convierten en variables numéricas antes de entrenar el modelo.

El proceso de entrenamiento del modelo:

- Se define el conjunto de características (X) y el objetivo (y) que se utilizarán para entrenar el modelo. Las características (X) se obtienen del DataFrame df_juegos y se seleccionan las columnas 'Genero', 'Plataforma' y 'Compañia_Desarrollo'.

- El objetivo (y) se obtiene del DataFrame df_juegos y se selecciona la columna 'Ventas_Globales'. Las características categóricas en X se convierten en variables numéricas utilizando la técnica de codificación one-hot mediante pd.get_dummies(X).

- Los datos se dividen en conjuntos de entrenamiento (X_train, y_train) y de prueba (X_test, y_test) utilizando la función train_test_split(). Se utiliza un tamaño de prueba del 20% y se establece una semilla aleatoria para garantizar la reproducibilidad de los resultados.

- Se crea un objeto de modelo de regresión lineal utilizando LinearRegression(). El modelo se entrena utilizando los datos de entrenamiento (X_train, y_train) mediante el método fit().

Variables utilizadas:

- X: El conjunto de características utilizado para entrenar el modelo. Incluye las columnas 'Genero', 'Plataforma' y 'Compañia_Desarrollo' del DataFrame df_juegos.
- y: El objetivo del modelo, que corresponde a las ventas globales de los videojuegos (columna 'Ventas_Globales' en df_juegos).


---


## 8.4.5 Validación del modelo

El proceso de validación del modelo:

- Se crea un nuevo DataFrame llamado ‘nuevo_juego’ que representa un nuevo juego con atributos para los cuales deseamos predecir las ventas globales.
- Los atributos categóricos del nuevo juego ('Genero', 'Plataforma', 'Compañia_Desarrollo') se convierten en variables numéricas utilizando la técnica de codificación one-hot mediante pd.get_dummies(nuevo_juego).
- El DataFrame nuevo_juego se reindexa para asegurarse de que todas las columnas sean las mismas que las utilizadas durante el entrenamiento del modelo. Esto se logra mediante reindex(columns=X_train.columns, fill_value=0), donde X_train es el conjunto de características utilizado para entrenar el modelo.
- Se utiliza el modelo entrenado (model) para predecir las ventas globales del nuevo juego utilizando el método predict(nuevo_juego).
- El valor de las ventas globales predichas se almacena en la variable ventas_predichas.
- Se imprime en pantalla el mensaje "Las ventas globales predichas para el nuevo juego son:" seguido del valor de ventas_predichas[0], que representa la predicción de ventas para el nuevo juego.

La validación del modelo se realiza de tal forma que se va a asignar nuevos valores a los atributos específicos y predecir de ventas del nuevo juego. Esto puede permitir obtener una estimación de las ventas globales del nuevo juego basada en el modelo entrenado.


## 8.4.6 Resultados del Modelo de Regresión

La predicción del modelo utilizando regresión lineal a partir de los atributos 'Genero', 'Plataforma' y    'Compañia_Desarrollo' da como resultado: 

**Las ventas globales predichas para el nuevo juego son: 0.1502685546875 de copias**

El modelo entrenado puede realizar predicciones sobre el éxito de un determinado género de juego en una plataforma específica. Estas predicciones pueden ayudar en la toma de decisiones sobre el tipo de género y plataforma a desarrollar el Serious Games.


---

## 8.4.7 Modelo de Regresión Logística

El modelo se define en los siguientes pasos:

- Predecir la probabilidad que un videojuego sea exitoso o no.
- Implementar el algoritmo de Regresión Logística: es un algoritmo que ajusta los coeficientes de la regresión para encontrar la mejor línea de separación entre las clases.
- El algoritmo va a predecir la probabilidad de clasificar correctamente los videojuegos como exitosos o no exitosos, va utilizar las variables 'Género', 'Plataforma' y 'Compañía de desarrollo'.
- Las variables las variables predictoras 'Género', 'Plataforma' y 'Compañía de desarrollo'.
- Definir las características 'Genero', 'Plataforma' y el objetivo 'Exitoso'.
- Ajustar los coeficientes de la regresión logística para maximizar la probabilidad de clasificar correctamente los videojuegos como exitosos o no exitosos.
- Calcular la media de las ventas globales y se utiliza como umbral para determinar qué juegos se considerarán exitosos.
- Crear una nueva columna llamada 'Exitoso' que indica si las ventas globales superan el umbral.
- Realizar la codificación one-hot de las columnas categóricas 'Genero' y 'Plataforma' utilizando el encoder OneHotEncoder de scikit-learn.
- Dividir los datos en conjuntos de entrenamiento y prueba.
- Crear el clasificador de regresión logística utilizando LogisticRegression.
- Entrenar el modelo utilizando los datos de entrenamiento.
- Predecir si un videojuego sea exitoso o no.
- Evaluar el rendimiento del modelo en la clasificación de los juegos como exitosos o no exitosos.


---

## 8.4.8 Entrenamiento del modelo

- Se realiza un preprocesamiento de los datos. Se multiplica la columna 'Ventas_Globales' por 1,000,000 para obtener las ventas globales en unidades más manejables. 

- Se calcula la media de las ventas globales y se utiliza como umbral para determinar qué juegos se considerarán exitosos.

- Se crea una nueva columna llamada 'Exitoso' que indica si las ventas globales superan el umbral.

- Se asignan las variables predictoras (X) y la variable objetivo (Y) a partir del DataFrame 'df_juegos'. Las variables predictoras son 'Genero' y 'Plataforma', y la variable objetivo es 'Exitoso'.

- Se realiza la codificación one-hot de las columnas categóricas 'Genero' y 'Plataforma' utilizando el encoder OneHotEncoder de scikit-learn. Esto es necesario para convertir las variables categóricas en variables numéricas que el modelo pueda entender.

- Se dividen los datos en conjuntos de entrenamiento y prueba utilizando la función train_test_split. En este caso, se asigna el 20% de los datos al conjunto de prueba y el 80% restante al conjunto de entrenamiento.

- Se crea el clasificador de regresión logística utilizando LogisticRegression de scikit-learn y se entrena el modelo utilizando los datos de entrenamiento (X_train, Y_train).

- Al tener entrenado el modelo, se realizan predicciones en los datos de prueba utilizando el método predict del clasificador. Las predicciones se almacenan en la variable 'Y_pred'.

- Se evalúa el modelo utilizando la función classification_report y confusion_matrix para obtener métricas de evaluación como la precisión, el recall, el F1-score y la matriz de confusión. Estas métricas permiten evaluar el rendimiento del modelo en la clasificación de los juegos como exitosos o no exitosos.

---

### 7.8.1 Validación del modelo

La validación del modelo se realiza utilizando técnicas de división de los datos en conjuntos de entrenamiento y prueba, y posteriormente evaluando el rendimiento del modelo en el conjunto de prueba.

En este caso, se ha utilizado el método train_test_split de la biblioteca scikit-learn para dividir los datos en un conjunto de entrenamiento (X_train, Y_train) y un conjunto de prueba (X_test, Y_test). El parámetro test_size=0.2 indica que se ha asignado el 20% de los datos al conjunto de prueba, mientras que el 80% restante se ha utilizado para el entrenamiento.

Después de dividir los datos, se ha creado un clasificador de regresión logística utilizando LogisticRegression de scikit-learn. Este clasificador se ha entrenado utilizando los datos de entrenamiento (X_train, Y_train).

Una vez entrenado el modelo, se han realizado predicciones en los datos de prueba utilizando el método predict del clasificador. Estas predicciones se han almacenado en la variable Y_pred.

Finalmente, se ha evaluado el modelo utilizando las métricas de evaluación classification_report y confusion_matrix. El classification_report proporciona información detallada sobre la precisión, el recall y el F1-score para cada clase, así como el soporte (número de instancias) de cada clase en el conjunto de prueba. La confusion_matrix muestra la matriz de confusión, que proporciona información sobre las predicciones correctas e incorrectas del modelo.


---

## 8.4.9 Resultados del Modelo de Regresión Logística

Los resultados en base al informe de clasificación:


- Precisión: La precisión es la proporción de predicciones positivas que fueron realmente correctas. En tu caso, la precisión para la clase "False" (no exitoso) es del 87%, lo que significa que el 87% de las predicciones de juegos no exitosos fueron correctas. Para la clase "True" (exitoso), la precisión es del 61%, lo que indica que el 61% de las predicciones de juegos exitosos fueron correctas.

- Recall: El recall, también conocido como sensibilidad o tasa de verdaderos positivos, es la proporción de casos positivos que fueron correctamente identificados por el modelo. En tu caso, el recall para la clase "False" es del 100%, lo que significa que el modelo identificó correctamente todos los juegos no exitosos. Sin embargo, el recall para la clase "True" es muy bajo, del 5%, lo que indica que el modelo no identificó adecuadamente la mayoría de los juegos exitosos.

- F1-score: El F1-score es una medida que combina tanto la precisión como el recall en una sola métrica. Es útil cuando hay un desequilibrio de clases. En tu caso, el F1-score para la clase "False" es del 93%, lo que indica un buen equilibrio entre precisión y recall. Sin embargo, el F1-score para la clase "True" es muy bajo, del 9%, lo que indica un rendimiento deficiente en la detección de juegos exitosos.

- Support: El "support" representa el número de muestras de cada clase en los datos de prueba.

- Accuracy: La precisión global del modelo en predecir correctamente ambas clases es del 87%. Sin embargo, debido al desequilibrio de clases, esta métrica puede ser engañosa.

- Matriz de confusión: La matriz de confusión muestra la distribución de las predicciones en cada clase. En tu caso, el modelo predijo correctamente 3109 juegos no exitosos y 22 juegos exitosos. Sin embargo, también hubo 456 juegos exitosos clasificados erróneamente como no exitosos y 14 juegos no exitosos clasificados erróneamente como exitosos.

Estos resultados sugieren que el modelo parece tener un buen desempeño en la clasificación de juegos no exitosos, pero un desempeño deficiente en la clasificación de juegos exitosos. Esto podría indicar que hay un desequilibrio de clases en los datos o que el modelo necesita ajustes o mejoras para detectar adecuadamente los juegos exitosos.


---

8.5 Predicción y toma de decisiones
Las predicciones de los diferentes modelos:

Resultados del Modelo de Clasificación: el modelo tiene problemas para predecir el género de los videojuegos basándose en las variables de entrada que se han utilizado.
Resultados del Modelo de Regresión Lineal: el modelo a partir de los atributos 'Genero', 'Plataforma' y 'Compañia_Desarrollo' da como resultado "las ventas globales predichas para el nuevo juego son: 0.1502685546875 de copias".
Resultados del Modelo de Regresión Logística: el modelo no tiene resultados satisfactorios, tiene dificultades para identificar correctamente los videojuegos exitosos.
Por lo que la toma de decisiones se basa en el Objetivo de proyecto y el resultado de los Modelos de datos, se decide que el modelo más adecuado para utilizar es el Modelo de Regresión Lineal, que se diseñó para predecir un valor numérico continuo (ventas globales).

En este caso, el modelo de regresión lineal fue el único que produjo una predicción directamente utilizable, al dar un valor de la cantidad de millones de copias al introducir los atributos:

'Genero': Ejemplo del valor a introducir ('Action').
'Plataforma': Ejemplo del valor a introducir ('PC').
'Compañia_Desarrollo': Ejemplo del valor a introducir ('Capcom').
Los modelos de clasificación y regresión logística, por otro lado, se utilizan para predecir categorías o clases, y en el contexto, se demostró tener dificultades para realizar predicciones precisas en el género de un videojuego o si un videojuego será exitoso o no.

Sin embargo, dada la baja precisión de los modelos, se puede explorar otras características del conjunto de datos o probar diferentes modelos (árboles de regresión, de soporte vectorial o las redes neuronales). Además, puede ser útil recolectar más datos, o intentar ajustar los parámetros de los modelos para mejorar la precisión de las predicciones.


# 9. Conclusión

En el análisis de los datos, se evaluaron tres tipos diferentes de modelos predictivos: un modelo de clasificación, un modelo de regresión lineal y un modelo de regresión logística. Cada uno de estos modelos tiene su utilidad y es útil en diferentes contextos.

Sin embargo, en base a los resultados obtenidos y al objetivo específico de este proyecto, se concluye que el modelo de regresión lineal es el más adecuado para predecir las ventas globales de un videojuego basado en atributos como el género, la plataforma y la compañía de desarrollo del juego. Los otros dos modelos, de clasificación y regresión logística, demostraron tener dificultades para realizar predicciones precisas en el contexto de este problema, ya que tuvieron problemas el primero para predecir el género de un videojuego y el segundo para predecir si un videojuego fuera exitoso.

A pesar de que se obtuvieron algunos resultados útiles, se hace evidente que hay margen para mejorar estos modelos. En concreto, sería útil explorar otras características que podrían influir en las ventas globales de un videojuego, como la fecha de lanzamiento del juego, las calificaciones recibidas por el juego, o incluso la presencia de ciertos personajes o temáticas en el juego. También puede ser útil probar con diferentes tipos de modelos, como los árboles de decisión, máquinas de soporte de vectores o redes neuronales artificiales, que pueden ser más eficaces en ciertos contextos.

Asimismo, sería beneficioso recolectar más datos y posiblemente ajustar los parámetros de los modelos para mejorar la precisión de las predicciones. Sin embargo, la recolección de datos adicionales siempre debe hacerse de manera ética y con el consentimiento adecuado, y debe tenerse en cuenta que ajustar demasiado los modelos puede llevar a un sobreajuste, donde el modelo se desempeña muy bien en los datos de entrenamiento, pero mal en los datos de prueba.

En resumen, aunque el modelo de regresión lineal fue el que dio los mejores resultados en este proyecto, hay mucho margen para mejorar y explorar otras opciones. El análisis de datos y la modelización son procesos iterativos, y siempre hay espacio para aprender, mejorar y probar nuevas ideas.


---

# 10. Bibliográfia

- Documentación oficial de Python: https://docs.python.org/3/
- Documentación oficial de Pandas: https://pandas.pydata.org/docs/
- Documentación oficial de Matplotlib: https://matplotlib.org/stable/contents.html
- Documentación oficial de Seaborn: https://seaborn.pydata.org
- Documentación oficial de Scikit-learn: https://scikit-learn.org/stable/
- Documentación oficial de Numpy: https://numpy.org/doc/stable/
- Analisis Exploratorio de Datos https://www.aprendemachinelearning.com/analisis-exploratorio-de-datos-pandas-python/
- Conceptos en Python https://www.geeksforgeeks.org
- Dudas https://stackoverflow.com/questions/tagged/pandas+python
- Analisis de datos https://ocw.uc3m.es/course/view.php?id=230
- Diccionarios de datos en data frame https://github.com/nsheikh23/COVID_StockMarket_Analysis/blob/master/52_Week.ipynb
- Procesamiento de data frames en pandas https://barcelonageeks.com/eliminar-una-o-varias-columnas-de-pyspark-dataframe/
- Data Clean https://github.com/mramshaw/Data-Cleaning
- Ploteo de datos https://github.com/tomimester/python-histogram/blob/master/plot-histogram-python-pandas.ipynb
- Data Cleaning in Python: the Ultimate Guide (2020) https://towardsdatascience.com/data-cleaning-in-python-the-ultimate-guide-2020-c63b88bf0a0d
- Regresión lineal en Python: un análisis detallado https://www.cienciadedatos.net/documentos/py10-regresion-lineal-python.html
- Aplicando Machine Learning para predecir éxitos de videojuegos https://www.saturdays.ai/projects/Videojuegos.html
- Machine Learning para la predicción de ventas https://www.aprendemachinelearning.com/regresion-lineal-en-espanol-con-python/
- McKinney, Wes. Python for Data Analysis. O'Reilly Media, Inc, 2017.
- VanderPlas, Jake. Python Data Science Handbook: Essential Tools for Working with Data. O'Reilly Media, Inc, 2016.











