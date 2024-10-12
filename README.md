# Obtain information on what type of Genre and Platform Serious Games can be developed
---
![Data Analysis](https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExbjZxaG9sMzFscnZ4a2Vkc2pxbWd3Y3g2eTNweDI2anNteXlidDdlNiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/doXBzUFJRxpaUbuaqz/giphy.webp)
---

## Author: Juan Carlos González Ibarra
## E-mail: jcgi.laboral@gmail.com
---

## Developed Date: june, 2023

---

## Content

1. Objectives
2. Development Methodology
3. Data Clean
4. Exploratory Data Analysis
5. Data Modeling
6. Results
7. Conclusion


---


---

# 1. Objectives

Oobtain valuable insights that support decision-making in determining the type of 'Genre' and/or 'Platform' for the development of Serious Games.

---

# 2. Development Methodology

To perform an **EDA** and **Data Modeling** that can help **establish the type of Genre and/or Platform for the Serious Games to be developed**, each task will be addressed as follows:

1. Definition of the _Target Variable(s)._

2. Data Cleaning:
   - Data Loading.
   - Data Preprocessing.
   - Remove irrelevant variables.
   - Impute missing values.
   - Clean attribute names that won’t be used.

3. Perform an EDA on the data to understand the distribution of the target variable(s) and variables needed to achieve the project's objective:

   - Correlation Analysis of Global Sales by Console and Genre.
   - Analysis of Global Video Game Sales by Platform.
   - Analysis of Global Sales by Genre.
   - Analysis of Global Sales by Development Company.

4. Generate a Supervised Predictive Model using Algorithms like:
   
   - Prediction: This algorithm is used for prediction. The key difference lies in the type of output variable being predicted.

5. Evaluate the model.

6. Implement the model.

7. Provide feedback on the model.

---

## 2.1 Definition of the Target Variable(s)

**The goal is to classify the 'Game Genre' and 'Platform',** either separately or together, to gather insights on the type of Genre and Platform to develop for Serious Games. Therefore, the correlation, classification, and prediction of the Game Genre and Platform will be based on the **analysis of successful video games**.

The **target variable** will be to determine which game genre and platform will be useful for creating a new successful video game. In this context, the **success of a video game** is defined **by the number of Copies Sold, as represented in the 'Global Sales' attribute**. Thus, the **variables** to be used to achieve the project's **objective** may include:

- **Game Genre:** This variable represents the category or type of game, such as action, adventure, strategy, sports, etc.

- **Platform:** This variable indicates the system or device on which the game will be released and played, such as PlayStation, Xbox, PC, Nintendo Switch, etc.

- **Global Sales:** This variable represents the total worldwide sales of the game. It will be **used as a success measure** to determine **whether a game is successful or not**.

- **Other Variables:** Other relevant variables for the analysis, such as game rating, review scores, development company, release date, etc., may also be considered depending on data availability and relevance to the specific objective.


---

# 3. Data Clean

## 3.1 Descripción de los datos

### In this project, a dataset was obtained through Web Scraping from the following websites:

*   [https://www.mobygames.com](https://www.mobygames.com)
    
*   [https://www.kaggle.com/datasets/sidtwr/videogames-sales-dataset](https://www.kaggle.com/datasets/sidtwr/videogames-sales-dataset)
    
*   [https://www.kaggle.com/datasets/gregorut/videogamesales](https://www.kaggle.com/datasets/gregorut/videogamesales)
    

The datasets are in CSV format and include:

*   consolas.csv
    
*   consolas2.csv
    
*   juegos\_mas\_vendidos.csv
    
*   vgsales.csv
    
*   video\_games.csv
    

The information contained in the CSV files is as follows:

### **consolas.csv & consolas2.csv**:

Contain information about gaming platforms, games developed, and reviews.

*   Attributes:
    
    *   **Platform**: This string attribute describes the name of the gaming console for which the games were developed.
        
    *   **Games\_x**: This integer attribute represents the number of games that have been developed for the specific console represented in the "Platform" column.
        
    *   **Player Reviews**: This integer attribute shows the number of reviews or critiques made by players about the console.
        
    *   **Critic Reviews**: This integer attribute shows the number of reviews made by professional critics about the console.
        
    *   **Companies**: This attribute combines text and integers to show the number of game development companies that have developed titles for the console.
        
    *   **Years**: This is a text string with integer values that indicates the range of years during which the console has been on the market. For example, a value of "2001 - 2020" would indicate that the console was released in 2001 and has been used up until 2020.
        

### **juegos\_mas\_vendidos.csv & vgsales.csv & video\_games.csv**:

Contain information on the best-selling games by platform, genre, etc., and statistics on the average time a player spends playing.

*   Attributes:
    
    *   **Title**: (String) The name of the video game.
        
    *   **Development Company**: (String) The company or studio that developed the video game.
        
    *   **Release Date**: (Int) The date the video game was officially released.
        
    *   **Genre**: (String) The type or category of the game (e.g., action, adventure, strategy, etc.).
        
    *   **Platform**: (String) The system or device on which the game was released and can be played (e.g., PlayStation, Xbox, PC, etc.).
        
    *   **Multiplatform**: (String) An indicator of whether the video game is available on more than one platform.
        
    *   **Portable**: (Bool) An indicator of whether the video game is available on portable platforms (e.g., Nintendo Switch, PSP, etc.).
        
    *   **Online**: (Bool) An indicator of whether the video game has online play functionality.
        
    *   **Max Players**: (Bool) The maximum number of players that can play the video game simultaneously.
        
    *   **Rating**: (Int) The age rating or recommendation for the video game (e.g., E for Everyone, T for Teens, M for Mature, etc.).
        
    *   **Ranking**: (Int) The game's ranking in a list, generally in terms of popularity or sales.
        
    *   **Review Score**: (Float) The average score or rating given to the video game by critics.
        
    *   **Sequel**: (Bool) An indicator of whether the video game is a sequel to a previous game.
        
    *   **Licensed**: (Bool) An indicator of whether the video game is based on an existing license (e.g., a movie, TV show, comic book, etc.).
        
    *   **Sales NA**: (Float) The number of copies of the video game sold in North America.
        
    *   **Sales EU**: (Float) The number of copies of the video game sold in Europe.
        
    *   **Sales JP**: (Float) The number of copies of the video game sold in Japan.
        
    *   **Sales Others**: (Float) The number of copies of the video game sold in other regions of the world.
        
    *   **Global Sales**: (Float) The total number of copies of the video game sold worldwide.
        
    *   **Estimated Sales**: (Float) An estimate of the total number of copies the video game will sell in the future, based on current sales trends.
        
    *   **Length.All PlayStyles.Average**: (Float) Represents the average game duration considering all play styles.
        
    *   **Length.All PlayStyles.Leisure**: (Float) Shows the game duration for players who enjoy the game more casually, covering all play styles.
        
    *   **Length.All PlayStyles.Median**: (Float) The median game duration, taking into account all play styles.
        
    *   **Length.All PlayStyles.Polled**: (Float) The number of observations or samples used to calculate the average game duration for all play styles.
        
    *   **Length.All PlayStyles.Rushed**: (Float) Reflects the game duration for players who progress through the game more quickly, considering all play styles.
        
    *   **Length.Completionists.Average**: (Float) The average game duration for completionist players who aim to achieve 100% of the game.
        
    *   **Length.Completionists.Leisure**: (Float) Shows the game duration for completionist players who play more casually.
        
    *   **Length.Completionists.Median**: (Float) The median game duration for completionist players.
        
    *   **Length.Completionists.Polled**: (Float) The number of observations or samples used to calculate the average game duration for completionists.
        
    *   **Length.Completionists.Rushed**: (Float) Represents the game duration for completionist players who progress through the game more quickly.
        
    *   **Length.Main + Extras.Average**: (Float) Shows the average game duration when playing the main story plus extra content.
        
    *   **Length.Main + Extras.Leisure**: (Float) The game duration for players who enjoy the main story and extra content more casually.
        
    *   **Length.Main + Extras.Median**: (Float) The median game duration, considering the main story and extra content.
        
    *   **Length.Main + Extras.Polled**: (Float) The number of observations or samples used to calculate the average game duration for the main story plus extras.
        
    *   **Length.Main + Extras.Rushed**: (Float) Reflects the game duration for players who progress through the main story and extras more quickly.
        
    *   **Length.Main Story.Average**: (Float) Shows the average duration of the game's main story.
        
    *   **Length.Main Story.Leisure**: (Float) Represents the duration of the game's main story for players who enjoy it more casually.
        
    *   **Length.Main Story.Median**: (Float) The median duration of the game's main story.
        
    *   **Length.Main Story.Polled**: (Float) The number of observations or samples used to calculate the average duration of the main story.
        
    *   **Length.Main Story.Rushed**: (Float) Indicates the duration of the main story for players who progress more quickly through it.
        

### Entity-Relationship Diagram
<img src="img/Proyecto_Final.png" width="600" height="400">

---


## 3.3 Preprocess the Data
-----------------------

### Merging DataFrames

Two DataFrames (df_consolas and df_consolas2) will be merged. The common attribute is "Platform," which represents the name of the platform on which the video game runs.

Three DataFrames (df_juegos, df_vgsales, df_video_games) will be merged. The common attributes are "Título" in df_juegos, "Name" in df_vgsales, and "Title" in df_video_games, which represent the name of the video game.

### Removing Irrelevant Variables

In the df_consolas DataFrame, the 'Games_y' attribute will be removed because it is a duplicate of 'Games_x'. The remaining attributes will be renamed as follows:

-   'Platform': 'Plataforma'
-   'Companies': 'Compañia'
-   'Games_x': 'Juegos_Desarrollados'
-   'Years': 'Anios'
-   'Player Reviews': 'Resenas_Jugador'
-   'Critic Reviews': 'Cantidad_Criticas'

All null values (NaN) in the DataFrame will be replaced according to the data type as follows:

-   'Plataforma' with 'Desconocido'
-   'Compañia' with 'Desconocido'
-   'Juegos_Desarrollados' with 0
-   'Anios' with 0
-   'Resenas_Jugador' with 0
-   'Cantidad_Criticas' with 0

In the df_juegos DataFrame, a broader data processing will be performed:

-   Null values in the 'Genre_x' column will be replaced with the corresponding values from the 'Genre_y' column.

-   The 'Genre_y' column will be deleted from the DataFrame since the null values in 'Genre_x' have been filled with the corresponding values.

-   The following columns will be removed: 'Fecha_Lanzamiento', 'Unnamed: 11', 'Fecha_Lanzamineto', 'Desarrollador_y', 'Genre', 'Desarrollador_x', and 'Distribuidor'.

-   The columns of the DataFrame will be renamed using a dictionary that specifies the new name for each column.

-   Columns will be reorganized for better clarity.

-   A list called 'columnas' will be defined, containing the names of the columns to be modified, and the iteration over each column in the list will replace their null values.

-   For string-type attributes, empty spaces will be replaced with 'Desconocido'.

-   A list called 'valores_incorrectos' ('2007', '2009', '2010', '2011', '2012', '2013', '2014', '2015') will be defined, containing values to be replaced in the 'Genero' attribute with 'Desconocido'.

-   For int or float-type attributes, empty spaces will be replaced with 0.

-   For bool-type attributes, empty spaces will be replaced with 'False'.

## 4 Exploratory Data Analysis (EDA)

In the exploratory analysis, the DataFrames are analyzed with the information provided in the previous section. The purpose is to analyze and investigate the datasets, summarize their main characteristics, identify relationships, understand the distribution of the target variable(s), and the variables to achieve the project’s objective.

The following is defined:

- #### Global Sales Analysis by Year.
- #### Correlation Analysis of Global Sales by Console and Genre.
- #### Global Sales Analysis of Video Games by Platform.
- #### Global Sales Analysis by Genre.
- #### Global Sales Analysis by Development Company.

---

## 4.1 Global Sales Analysis by Year.

In this analysis, the distribution of global video game sales over the years is examined using the 'Release_Date' attribute, which contains the launch date information, and the 'Global_Sales' attribute, which contains the total global sales of the video game. The relationship between global sales and the year of release is visualized in a line chart.
The goal is to identify patterns or trends in sales over time, such as peaks or declines in certain years. This can help understand the evolution of the video game industry and make strategic decisions based on historical sales.

---

### 6.1.1 Relevant Information:

- The average global sales amount to 500,000 copies over a span of 37 years.
- The highest sales peaks occurred between 2007 and 2008.
- Sales began to increase in 2000 but started declining after 2015.

---

## 4.2 Correlation Analysis of Global Sales by Console and Genre.

We can explore the correlations between the various attributes present in the df_juegos DataFrame to better understand their relationships and select features for data modeling.

The correlation matrix is a table showing the correlation coefficient (also known as Pearson's r) between pairs of variables in a dataset. Each cell of the table displays the correlation between two variables.

The features of the correlation matrix are:

- The correlation coefficient is a statistical measure that describes the degree of relationship between two variables.
- The correlation coefficient ranges from -1 to +1.
- A correlation of +1 indicates a strong positive correlation, meaning the two variables tend to increase together.
- A correlation of -1 indicates a strong negative correlation, meaning that as one variable increases, the other decreases.
- A correlation of 0 indicates no linear relationship between the variables.

---

By visualizing the correlation matrix with a heatmap, one can get a view of how the variables in the df_juegos dataset are correlated.

In the heatmap:

- Colored cells represent the correlations between variables.
- The color of each cell is determined by the correlation value and the color map used.
- Strong correlations (close to 1 or -1) are indicated by more intense colors, while weak correlations (close to 0) are shown with lighter colors.

**A strong positive correlation is observed between 'Global_Sales', 'Ranking', and 'Review_Score', suggesting that video games with higher review scores tend to have more global sales. This implies that the quality of a game (as measured by reviews) may influence its commercial success. However, correlation does not imply causation, and more research is needed to understand the relationship between these variables.**

---

### 4.2.1 Relationship Between Genre and Global Sales**

To delve deeper into the correlation analysis, a graph is generated showing the relationships between three variables: 'Platform', 'Global_Sales', and 'Genre'. The 'Platform' variable is displayed along the x-axis, 'Global_Sales' along the y-axis, and 'Genre' is represented by the color of the points.

Thus, each point on the graph represents a game, and its position on the x and y axes indicates the platform on which the game was released and the global sales it achieved. The color of the point indicates the genre of the game.

The graph shows how global sales vary based on the platform and genre.

---

If points of a specific color (representing a certain genre) are clustered in a specific area of the graph, it suggests that the genre tends to have more sales on certain platforms.

### 4.2.2 Relevant Information:
- **The average global sales for each genre are below 10 million copies, so it's suggested to analyze the average global sales by genre and/or platform.**
- The genres with the highest sales are Action, Racing, Platform, Role Playing, and Shooter.
- The platforms with the highest sales by genre are:
  - Action (Nintendo, PlayStation, and Xbox).
  - Racing (Nintendo, PlayStation, and Xbox).
  - RPG (Nintendo, PlayStation, and Xbox).
  - Shooter (PlayStation and Xbox).

---

## 4.3 Global Sales Analysis of Video Games by Platform.

As a result of the previous correlation analysis, the relationship between 'Global_Sales', 'Genre', and 'Platform' is observed to be below 1 million copies. Therefore, an analysis of the average 'Global_Sales' will be conducted.

This analysis examines the distribution of video game sales according to the platform they are played on, using the 'Platform' attribute (which contains information on the platform) and the 'Global_Sales' attribute (containing the total global sales). The total sales by platform are calculated and visualized in a line chart, highlighting each maximum point in the 'Platform' attribute for the most popular or successful video games in terms of sales. This can help understand the console market and make decisions on developing and distributing games for specific platforms.

---

### 4.3.1 Relevant Information:
- The average global sales per platform are below 1 million copies.
- The total average global sales for all platforms is 548,394 million copies.
- The platforms with the highest sales are Nintendo, PlayStation, and Xbox.

---

## 4.4 Global Sales Analysis by Genre.

In this analysis, the distribution of global video game sales is examined using the 'Genre' attribute (which contains information on the genre of the video game) and the 'Global_Sales' attribute (which contains the total global sales of the video game). The total sales by genre are calculated and visualized in a line chart, highlighting each maximum point in the 'Genre' attribute for the most popular or successful video games in terms of sales. This can provide useful insights for making decisions related to the development and marketing of new games and for understanding players' preferences and interests.

---

### 4.4.1 Relevant Information:
- The average global sales by genre are below 1 million copies.
- The total average global sales for all genres is 548,394 million copies.
- The genres with the highest sales are:
  - Arcade.
  - Sandbox.
  - Platform.
  - Shooter.
  - RPG.
  - Racing.
  - Sports.
  - Action.

---

## 4.5 Global Sales Analysis by Development Company.

This analysis examines the distribution of global video game sales by the company that developed the games, using the 'Development_Company' attribute (which contains information on the company that developed the video game) and the 'Global_Sales' attribute (which contains the total global sales of the video game). The total sales by company are calculated and visualized in a line chart. The goal is to identify which development companies have the most success in terms of video game sales. This can be useful for evaluating the reputation and performance of development companies and for making decisions about partnerships or acquisitions in the industry.

---

### 4.5.1 Relevant Information:

Most development companies have an average global sales below 500,000 copies.
The development companies with the highest sales are:
- Nintendo.
- Electronic Arts.
- Activision.
- Sony.
- Ubisoft.

---

### 4.6 AED Results

To link the analyses to data modeling, the strengths of each type of analysis are summarized according to the project’s objective:



- **Correlation Analysis of Global Sales by Console and Genre:**

  - The correlation between the attributes in the df_juegos DataFrame can be examined.
  - A positive correlation between 'Global_Sales', 'Ranking', and 'Review_Score' can be identified.
  - Video games with higher review scores tend to have more global sales, which can be used as a target variable to define Serious Games, considering the reviews and ranking that the player can achieve, and how this can enhance the educational experience.
  - In conclusion, this data can be used to determine which genre of video game should be used to develop Serious Games.
  
  
  
- **Global Sales Analysis of Video Games by Platform:**

  - The distribution of video game sales by platform or console can be examined.
  - The most popular platforms in terms of sales can be identified.
  - It is possible to evaluate which platforms are most suitable for Serious Games, considering the technical characteristics and usability required to offer an effective educational experience.
  - In conclusion, this data can be used to determine which platforms should be used to develop and distribute Serious Games.
  
  
  

- **Global Sales Analysis by Genre:**

  - The distribution of video game sales by genre can be examined.
  - The most popular video game genres in terms of sales can be identified.
  - It is possible to evaluate which genres are relevant for Serious Games, considering the educational or informative goal of the game.
  - In conclusion, this data can be used to determine which genre of Serious Games has the highest potential for acceptance and success in the market.
  
  
  

- **Global Sales Analysis by Development Company:**

  - The distribution of video game sales by development company can be examined.
  - The companies with a successful track record in terms of video game sales can be identified.
  - Possible partnerships or collaborations with these companies for the development and distribution of Serious Games can be evaluated.
  - In conclusion, this data can be used to select a development company with experience in the chosen genre and platform.




By combining these analyses, a more comprehensive and data-backed view of the most suitable genre and platform for developing Serious Games can be obtained. These


---

5. Data Modeling


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











