# Proyecto final de Ciencia de Datos
## Introducción
En este proyecto se desarrolló un modelo de regresión lineal múltiple para analizar los factores que influyen en el precio de propiedades publicadas en Airbnb.
## Objetivo
Aplicar técnicas de regresión lineal múltiple para analizar el mercado inmobiliario de Airbnb y desarollar un modelo predictivo que permita estimar precios a partir de distintas variables relacionadas con las propiedades.
## Dataset utilizado
El dataset contiene información muy variada sobre las propiedas de Airbnb, incluyendo variables como la capacidad, la ubicación o la reputación del alojamiento.
## Limpieza de datos
### Librerias utilizadas
Para la limpieza se utilizaron las siguientes librerias
* Pandas
* Numpy
* Matplotlib
* Seaborn

### Carga y exportación del dataset
Se cargo el dataset y se comenzaron a analizar los valores nulos, encargandose de mantener solo la información relevante, y también asegurando que valores atípicos extremos no afecten negativamente al modelo. Una vez ya limpiado se exporta el dataset para su modelado

## Analisis exploratorio
### Pairplot
Obtuvimos varias observaciones importantes basadas en las relaciones entre variables, por ejemplo la relación de variables de tamaño y capacidad con respecto al precio.
También se identificó dispersión considerable, indicando que el precio depende de múltiples factores y no únicamente de una sola variable.

### Mapa de correlación
El mapa de correlación permitió identificar relaciones lineales entre las variables numéricas, que moderadamente positivas entre sí.

### Construcción del modelo
La variable dependiente fue log_price y las variables independientes se seleccionaron a partir de las características relevantes del dataset. Se transformaron variables de texto en numéricas para hacerlas compatibles con el modelo de regresión. Se dividen los datos en entrenamiento y prueba.

### Entrenamiento del modelo
El modelo se entrena utilizando las variables seleccionadas y posteriormente se utiliza para generar predicciones

### Evaluación del modelo
El coeficiente r2 se utiliza para medir el porcentaje de variabilidad del precio explicado por el modelo.

El ajuste de r2 permite evaluar el desempeño considerando la cantidad de variables utilizadas, ayudando a evitar interpretaciones engañosas relacionadas al exceso de variables.

Finalmente el error cuadrático medio permitio medir el nivel promedio de error en las predicciones realizadas, mientras menor sea, mejor es la predicción.

### Predicciones vs valores reales
La gráfica mostró una tendencia positiva consistente, lo que indicó que el modelo logró aproximarse al comportamiento real de los precios.

### Resultados
El modelo logró identificar patrones relevantes en el comportamiento del precio, estimar precios de forma razonable y explicar parte importante de la variabilidad observada en el dataset