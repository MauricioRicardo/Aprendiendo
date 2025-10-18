# Modelo Relacional

El modelo relacional, para el modelado y la gestión de bases de datos, es un modelo de datos basado en la lógica de predicados y en la teoría de conjuntos.

Tras ser postuladas sus bases en 1970 por Edgar Frank Codd, de los laboratorios IBM en San José (California), no tardó en consolidarse como un nuevo paradigma en los modelos de base de datos.

Su idea fundamental es el uso de relaciones. Estas relaciones podrían considerarse en forma lógica como conjuntos de datos llamados tuplas. Pese a que esta es la teoría de las bases de datos relacionales creadas por Codd, la mayoría de las veces se conceptualiza de una manera más fácil de imaginar, pensando en cada relación como si fuese una tabla que está compuesta por registros (cada fila de la tabla sería un registro o “tupla”) y columnas (también llamadas “campos”).

Es el modelo más utilizado en la actualidad para modelar problemas reales y administrar datos dinámicamente.

El modelo relacional desarrolla un esquema de base de datos (data base schema) a partir del cual se podrá realizar el modelo físico o de implementación en el DBMS.

Este modelo esta basado en que todos los datos están almacenados en tablas (entidades/relaciones) y cada una de estas es un conjunto de datos, por tanto una base de datos es un conjunto de relaciones. La agrupación se origina en la tabla: tabla -> fila (tupla) -> campo (atributo)

El Modelo Relacional se ocupa de:
* La estructura de datos
* La manipulación de datos
* La integridad de los datos

Donde las relaciones estan formadas por :
* Atributos (columnas)
* Tuplas (Conjunto de filas)

Existen dos formas para la construcción de modelos relacionales:
* Creando un conjunto de tablas iniciales y aplicando operaciones de normalización hasta conseguir el esquema más óptimo,
* O, convertir el modelo entidad relación (ER) en tablas, con una depuración lógica y la aplicación de restricciones de integridad.

![](https://res.cloudinary.com/dtzgksveo/image/upload/v1689808582/PitooPlumo/SQL/Modelo-Relacional_wagvxi.png)

[Para mas informacion dar clic en este link](https://bookdown.org/paranedagarcia/database/nosql.html)

[Regresar](./Elementos.md)