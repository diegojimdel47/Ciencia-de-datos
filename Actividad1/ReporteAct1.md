# Actividad 1
## Perfiles de ciencias de datos
### Ingeniero de datos
Deportiva MX necesita priorizar el diseño de una infraestructura de datos capaz de organizar y almacenar grandes volúmenes de datos de forma eficiente y escalable, tarea en la que se especializa el ingeniero de datos.
### Analista de datos
Los datos obtenidos requieren ser interpretados para entender el comportamiento de las ventas y de los clientes, lo que permitirá una mejor toma de decisiones para la empresa.
### Científico de datos
Una vez organizados e interpretados, los datos nos permiten hacer predicciones de comportamientos futuros, esto con el objetivo de prevenir el desorden que un crecimiento de los datos y una falta de infraestructura pueden provocar.
## Las cinco V
### Volumen
Actualmente se esta experimentando un gran crecimiento de datos en la empresa, particularmente en los registros de venta, usuarios y productos. Esta situación necesita de soluciones para almacenar grandes cantidades de volúmenes de datos sin afectar el rendimiento.
### Velocidad
Los datos que se estan generando vienen en un fujo constante y veloz, por ello, es necesario desarrollar sistemas que permitan procesar y analizar la información de forma rápida para no interrumpir, más bien, adaptarse a este flujo.
### Variedad
Deportiva MX maneja varios tipos de datos, como información estructurada, semiestructurada o no estructurada. Esta variedad exige tecnologías capaces de adaptarse a diversos formatos.
### Veracidad
Esto es fundamental para la toma de decisiones, ya que se necesita que sean datos de calidad, confiabilidad, se puedan manejar errores, duplicados o información incompleta.
### Valor
Con esto nos referimos a transformar los datos en información útil, que permita mejorar la experiencia del cliente, optimizar procesos y aumentar las ventas.
## Arquitectura de almacenamiento
### Problemática
La problemática actual de la empresa se puede resumir en el crecimiento acelerado de datos, combinado con una falta de infraestructura adecuada, lo que impide aprovechar estos datos para la toma de decisiones y la optimización de los procesos. 
### Solución
La propuesta pensada para esta situación necesita de los siguientes componentes:
* Data Lake:

    Es donde se van a almacenar todos los grandes volúmenes de datos en su formato original, es decir, si son estructurados, semiestructurados o no estructurados.
* Base de datos NoSQL:

    Estaremos usando MongoDB que nos va permitirá gestionar los datos que se usan a diario, que posteriormente son almacenados en el Data Lake.

### Implementación de la solución
El flujo de datos dentro de la arquitectura sería la siguiente:
 1. Los datos como ventas, usuarios o productos son generados.
 2. Se almacenan en MongoDB para su uso diario.
 3. Posteriormente estos pasan al Data Lake para ser almacenados.
 4. Una vez ya almacenados, los datos se pueden procesar y limpiar para asegurar su calidad.
 5. Finalmente con la información limpia y filtrada, se utilizan herramientas de análisis para apoyar la toma de decisiones.
## Colecciones JSON
Como ya lo establecimos, usaremos MongoDb, que es una base de datos NoSQL, con colecciones que nos permitan almacenar la información de manera accesible y escalable.
### Usuarios
Contiene información básica de los clientes, como su nombre y correo electrónico.
### Productos
Incluye los productos disponibles, con datos como nombre y precio.
### Ventas
Registra las compras realizadas, relacionando a los usuarios con los productos.
### Diseño
```json
{
    "usuarios": [
        {
            "_id": "1",
            "nombre": "Juan",
            "email": "juan@gmail.com"
        }
    ],
    "productos": [
        {
            "_id": "101",
            "nombre": "Balón",
            "precio": 300 
        }
    ],
    "ventas": [
        {
            "_id": "500",
            "usuario_id": "1",
            "producto_id": "101",
            "cantidad": "2"
        }
    ]
}
```