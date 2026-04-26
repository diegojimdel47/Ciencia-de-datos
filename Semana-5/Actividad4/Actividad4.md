# Actividad 4
## Objetivo
Desarrollar y evaluar dos modelos supervisados:
1. Regresión lineal múltiple para estimar el precio de vehículos
2. Regresión logística binaria para predecir la superviviencia en el Titanic

## Parte 1 - Regresión lineal múltiple
### Preparación de los datos
Se seleccionaron las variables relevantes y se limpiaron los datos, asegurando que fueran númericos y sin valores faltantes.
### Análisis exploratorio
El pariplot mostró que el kilometraje tiene una relación negativa con el precio , mientras que el año tiene una relación positiva, lo cual coincide con el resultado esperado.
### Modelado
Se usaron el kilometraje y el año como las variables independientes, mientras que la dependiente fue el precio.
### Evaluación y validación
El modelo se evaluó con R2 y el error cuadrático medio, mostrando un ajuste adecuado. Además, los análisis de VIF y Durbin-Watson indican que no hay problemas importantes de multicolinealidad ni dependencia en los errores.
### Conclusión
El modelo refleja correctamente la relación entre las variables, aunque su precisión es limitada por la falta de más factores que influyan en el precio.

## Parte 2 - Regresión logística lineal
### Preparación de los datos
Se trabajó con variables como clase, sexo, edad y tarifa, elminando valores nulos y transformando las variables categóricas a fortmato numérico.
### Análisis 
Las visualizaciones y el t-test mostraron diferencias entre los grupos, indicando que algunas variables influyeron en la supervivencia.
### Modelado e interpretación
Se aplicó la regresión logísitca apra estimar la probabilidad de sobrevivir. La razón de momios perimitió identificar que variables aumentan o disminuyen esta probabilidad.
### Evaluación
El modelo se evaluó con exactitud, matriz de confusión y curva ROC, mostrando un desempeño adecuado en la clasificación.
### Conclusión
Variables como el sexo, la clase y la tarifa tienen un impacto importante en la supervivencia. El modelo es funcional, aunque como siempre, puede mejorar con más información.

## Conclusión general
Ambos modelos muestran como distintas técnicas se aplican dependiendo del tipo de problema. La calidad de los datos y la selección de variables son clave para lograr buenos resultados.