# Comandos

## SELECT
Se utiliza para recuperar datos de una o más tablas. Puedes usar esta cláusula para seleccionar todas las columnas de una tabla o solo las columnas específicas que necesitas.
```SQL
SELECT columnas
FROM nombre_tabla
WHERE condicion;
```

## INSERT
Se utiliza para agregar nuevos registros (filas) a una tabla. Puedes usarlo de varias formas dependiendo de tus necesidades
```SQL
INSERT INTO nombre_tabla (columna1, columna2, columna3, ...)
VALUES (valor1, valor2, valor3, ...);
```
```SQL
INSERT tabla (colum1, colum2, colum3)
VALUES (val1, val2, val3),(val4, val5, val6)
---> Inserta diferentes registro separados por una coma
```
```SQL
[INSERT INTO SELECT] = Copia datos de una tabla y los inserta en otra tabla
INSERT INTO tabla2 SELECT * FROM tabla1 WHERE condicion
INSERT INTO tabla2(col1, col2, col3) SELECT col1, col2, col3
FROM tabla1 WHERE condicion ---> Copia solo algunas columnas
```

## UPDATE
Actualizar los datos
```SQL
UPDATE tabla
SET columna1 = valor1, columna2 = valor2
WHERE condicion
```

## DELETE
Elimina registros 
```SQL
DELETE FROM tabla WHERE condicion
```

## Crear Base de Datos
```SQL
CREATE DATABASE NOMBRE
```

## Crear Tabla
```SQL
CREATE TABLE NOMBRE
    NOMCOLUMNA1 INT NOT NULL,
    NOMCOLUMNA2 VARCHAR(50) NOT NULL,
    NOMCOLUMNA3 DATE NULL,
    NOMCOLUMNA4 DATETIME NOT NULL,
    NOMCOLUMNA5 CHAR(3) NULL,
    CONSTRAINT PK_NOMCOLUMNA1 PRIMARY KEY (NOMCOLUMNA1)
```

## Identity y Primary Key
```SQL
CREATE TABLE NOMBRE
    NOMCOLUMNA1 INT IDENTITY (1,1) NOT NULL PRIMARY KEY,
```


## SP_HELP
Notifica información sobre un objeto de base de datos (cualquier objeto enumerado en la vista de compatibilidad sys.sysobjects ), un tipo de datos definido por el usuario o un tipo de datos.
```SQL
sp_help nombretabla
```

## SP_HELPTEXT
Muestra la definición de una regla definida por el usuario, el procedimiento almacenado de Transact-SQL sin cifrar, la función Transact-SQL definida por el usuario, el desencadenador, la columna calculada, la restricción CHECK, la vista o el objeto del sistema, como un procedimiento almacenado del sistema.
```SQL
sp_helptext nomprocesoalamacenado
```

## ALTER TABLE
Modifica una definición de tabla mediante la alteración, adición o retirada de columnas y restricciones. ALTER TABLE también vuelve a asignar y compilar particiones, o deshabilita y habilita restricciones y desencadenadores.

```SQL
ALTER TABLE Paciente ADD Estado	SMALLINT
ALTER TABLE Paciente ALTER COLUMN Estado BIT
ALTER TABLE Paciente DROP COLUMN Estado

ALTER TABLE Paciente 
ADD FOREIGN KEY(idPais) REFERENCES Pais(idpais)

ALTER TABLE HistorialPaciente
ADD FOREIGN KEY(idPaciente) REFERENCES Paciente(idPaciente)
```

## DROP TABLE
Quita todas las filas de una tabla o las particiones especificadas de una tabla, sin registrar las eliminaciones individuales de filas. TRUNCATE TABLE es similar a la instrucción DELETE sin una cláusula WHERE; no obstante, TRUNCATE TABLE es más rápida y utiliza menos recursos de registros de transacciones y de sistema.

```SQL
TRUNCATE TABLE NomTabla
```

## UNION
Concatena los resultados de dos consultas en un único conjunto de resultados. Puede controlar si en el conjunto de resultados se incluyen filas duplicadas:

* UNION ALL: incluye duplicados.
* UNION: se excluyen los duplicados.

Una operación de UNION es distinta de una operación de JOIN :

* Una operación de UNION concatena conjuntos de resultados de dos consultas. Pero una operación de UNION no crea filas individuales de columnas obtenidas de dos tablas.

* Una operación de JOIN compara las columnas de dos tablas para crear filas de resultados compuestas de columnas de las dos tablas.

A continuación, se muestran las reglas básicas para combinar los conjuntos de resultados de dos consultas con UNION:

* El número y el orden de las columnas debe ser el mismo en todas las consultas.

* Los tipos de datos deben ser compatibles.

```SQL
SELECT columnas FROM tabla1
UNION
SELECT columnas FROM tabla2;
```
[Regresar](./Conceptos.md)