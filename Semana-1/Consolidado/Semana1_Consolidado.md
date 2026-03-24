# Semana 1
## Actividad 1 (Completa) 
[Ir al reporte de la Actividad 1](../Actividad1/ReporteAct1.md)
### Resumen de la actividad
Se realizo una consultoría a la empresa Deportiva MX, la cual tuvo un incremento de datos que no se pudo manejar inicialmente, asi que se analizó la situación desde estos puntos:
1. Perfiles de ciencia de datos: Aquí consultamos cuales perfiles se adaptan a la situación de la empresa y como utilizarlos.
2. Las Cinco V: Con esto se analiza lo que la empresa tiene que tener en cuenta en base a sus datos, para entender su comportamiento.
3. Arquitectura de almacenamiento: Se propuso almacenar los datos primero en MongoDB para su uso operativo y diario, que después pasa a un Data Lake donde se almacena sin modificar su formato original.
4. Colecciones JSON: Por último se hizo el diseño básico de las colecciones de datos, diviendo entre usuarios, productos y ventas:
    * Usuarios: Aqui estan los datos como el nombre y el email del usuario.
    * Productos: En esto ponemos en nombre y el precio del producto.
    * Ventas: Para terminar, aqui se muestra la relación entre producto y venta.
### Colecciones JSON
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
## Propuesta de actividades (Incompleta)
## Ejercicios complementarios (Incompletos)