# Proyecto final
## Introducción
El precio de los alojamientos en Airbnb depdende de varios factores como la ubicación, el tamaño, el tipo de propiedad, servicios o la reputación del propietario. En el proyecto se realizo un modelo de predicción para analizar las variables más influyentes en el precio de los alojamientos.
## Dataset utilizado
El dataset contiene información sobre propiedades de Airbnb, algunas variables son:
* Tipo de propiedad
* Tipo de habitación
* Número de habitaciones
* Capacidad de huéspedes
* Ciudad
* Coordenadas geográficas
* Calificaciones
* Políticas de cancelación

La variable objetivo fue el logaritmo del precio

## Limpieza de datos
Se realizaron procesos como:
* Eliminación de valores nulos
* Imputación de datos numéricos y categóricos
* Conversión de formatos
* Revisión de inconsistencias
* Tratamiento de valores extremos

Posteriormente se generó un dataset limpio para entenar al modelo

## Variables selecionadas
Las variables fueron:
* Capacidad de huéspedes
* Número de baños
* Número de habitaciones
* Número de camas
* Tarifa de limpieza
* Número de reseñas
* Calificación promedio
* Tasa de respuesta del anfitrión
* Latitud
* Longitud
* Tipo de propiedad
* Tipo de habitación
* Tipo de cama
* Política de cancelación
* Ciudad
* Reserva inmediata imposible

## Análisis exploratorio
### Pairplot
El pairplot mostró relaciones positivas entre:
* Capacidad de huéspedes
* Número de baños
* Número de habitaciones
* Número de camas
* Precio

## Mapa de correlación
El mapa permitió identificar:
* Relaciones entre variables numéricas
* Posibles casos de multicolinealidad

Las variables relacionadas con tamaño mostraron correlaciones moderadamente positivas

## Construcción del modelo
Se utilizó un modelo de regresión lineal múltiple, donde se hizo:
* Codificación de variables categóricas
* División de los datos
* Evaluación mediante técnicas de regresión

## Evaluación del modelo
Las métricas utilizadas fueron:
* R2
* R2 ajustado
* Error cuadrático medio

Lo que permitió evaluar: 
* La capacidad predictiva
* El ajuste del modelo
* Nivel de error

## Predicciones vs valores reales
La gráfica mostró una tendencia positiva entre los valores reales y las predicciones, lo que indica que el modelo logró capturar patrones importantes en los datos

## Importancia de variables
El análisis de coeficientes mostró que:
* El tipo de propiedad
* La ubicación
* El tamaño del alojamiento

Influyen considerablemente en el precio final

## Multicolinealidad
Se calculo el Factor de Inflación de la Varianza o VIF, para detectar relaciones excesivas entre variables independitnes. Pero el modelo presentó niveles aceptables de multicolinealidad

## Conclusiones
* El modelo logró explicar una parte importante de la variabilidad del precio
* Las variables relacionadas con tamaño y ubicación fueron las más influyentes
* La regresión lineal múltiple permitió identificar los patrones relevantes
* Puede que teniendo más variables se mejoré la eficiencia del modelo