![Imagen no disponible por el momento](https://res.cloudinary.com/dtzgksveo/image/upload/v1701888522/PitooPlumo/SQL/Join_rcs8ub.png "Explicación grafica de Joins")

## INNER JOIN
INNER JOIN es una cláusula que se utiliza para combinar filas de dos o más tablas basándose en una condición de coincidencia entre las columnas de esas tablas. El resultado es un conjunto de resultados que contiene solo las filas que cumplen con la condición especificada.

```SQL
SELECT columnas
FROM tabla1
INNER JOIN tabla2 ON tabla1.columna = tabla2.columna;
```
## LEFT JOIN
La cláusula LEFT JOIN en SQL Server se utiliza para combinar filas de dos o más tablas basándose en una condición de coincidencia, y además incluye todas las filas de la tabla izquierda (la primera mencionada) en el resultado, incluso si no hay coincidencias en la tabla derecha.

```SQL
SELECT columnas
FROM tabla1
LEFT JOIN tabla2 ON tabla1.columna = tabla2.columna;
```

## RIGHT JOIN
 Se centra en todas las filas de la tabla derecha (la segunda mencionada), incluso si no hay coincidencias en la tabla izquierda. De manera similar a LEFT JOIN, se incluirán todas las filas de la tabla derecha en el resultado, y si hay coincidencias con la tabla izquierda, se mostrarán los datos correspondientes. Si no hay coincidencias, los valores de la tabla izquierda serán nulos.

 ```SQL
SELECT columnas
FROM tabla1
RIGHT JOIN tabla2 ON tabla1.columna = tabla2.columna;
 ```
[Regresar](Conceptos.md)