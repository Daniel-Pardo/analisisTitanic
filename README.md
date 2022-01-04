# Análisis: Titanic - Machine Learning from Disaster

## Autor
Daniel Pardo Navarro

## Descripción  

El hundimiento RMS Titanic en 1912 es uno de los naufragios más conocidos de la historia. El Titanic era un transatlántico británico considerado insumergible que en el momento de finalizar su consrucción era el mayor barco de pasajeros del mundo. No obstante, en su viaje inaugural desde Southampton a Nueva York se hundió después de chocar con un iceberg durante la noche del 14 y la madrugada del 15 de abril de 1912. Desgraciadamente, no existían suficentes botes salvavidas para todas las personas que vijaban y murieron 1502 personas de las 2224 totales que había etre pasajeros y la tripulación.

En este proyecto se utiliza el conjunto de datos *Titanic - Machine Learning from Disaster* que contiene muestras etiquetadas con las caracterísitcas de las personas y si sobrevivió al naufragio o no. El dataset que se utiliza corresponde a una competición activa de Kaggle que se encuentra disponible en https://www.kaggle.com/c/titanic/ y se realizará una fase preprocesado, análisis de los datos y generación de modelos de clasificación. 

## Ficheros

- code: Carpeta con el código en R y las salidas que se generan
    - PRA_2.Rmd: Contiene el código y el texto donde se desarolla todo el proyecto en RMarkdown. 
    - PRA_2.html: Salida en formato html del código. 

Datasets:
- train.csv: Conjunto con los datos de entrenamiento originales. 
- test.csv: Conjunto con los datos de test originales. 
- kaggle_rl.csv : Archivo con la predicción realizada mediante Regresión Logística
- kaggle_c50.csv: Archivo con la predicción realizada con el algoritmo C5.0
- kaggle_rf.csv: Archivo con la predicción realizada con Random Forest
- kaggle_svm.csv: Archivo con la predicción realizada con Support Vector Machine




## Conjunto de datos

El conjunto de datos orignal cuenta con las siguiente 12 variables: 

**PassengerId** - Identificador único para cada registro de un pasajero. 

**Survived** - Variable objetivo para clasificar la supervivencia de los pasajeros donde 0 = No sobrevivió y 1 = Sobrevivió

**Pclass** - Clase del billete del pasajero donde 1 = Primera clase, 2 = Segunda clase, 3 = tercera clase. 

**Name** - Nombre del pasajero. 

**Sex** - Sexo del pasajero que puede ser male (masculino) o female (femenino).

**Age** - Edad del pasajero en años. En caso de ser menor que 1 la edad es fraccionaria. Por ejemplo, en el caso de  0.42 sería 0.42*365=153,3 días. La edad, por lo tanto, podría ser desde 152/365 hasta 155/365

**SibSp** - Número de hermanos o cónyuges que viajan con cada pasajero.

**Parch** - Número de padres/niños que viajan. Si un niño viaja con una cuidadora este número será = 0.

**Ticket** - Número de billete. 

**Fare** - Cantidad de dinero que ha pagado el pasajero por el viaje.

**Cabin** - Número de cabina del pasajero.

**Embarked** - Puerto desde donde se embarcó / abordó el pasajero en particular donde C = Cherbourg, Q = Queenstown, S = Southampton

