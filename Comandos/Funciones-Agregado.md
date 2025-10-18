# Funciones de Agregado

## MAX
Maximo 
```SQL
SELECT MAX (columna) 
FROM tabla 
WHERE condicion
 ---> Muestra el valor mayor de columna
SELECT Columna2, MAX (columna1)
FROM tabla
GROUP BY Columna2
 ---> Muestra agrupado el valor mayor de una columna
```
## MIN
Minimo
```SQL
SELECT MIN (columna)
FROM tabla
WHERE condicion
---> Muestra el valor menor de columna
SELECT Columna2, MIN (columna1)
FROM tabla
GROUP BY Columna2
 ---> Muestra agrupado el valor menor de una columna
```
## SUM
Suma los valores
```SQL
SELECT SUM(columna) 
FROM tabla 
WHERE condicion
---> Suma los valores de la columna
SELECT Columna2, SUM(columna1)
FROM tabla
GROUP BY Columna2
---> Muestra agrupado el valor de la columna sumados
```
## AVG
Muestra el promedio
```SQL
SELECT AVG(columna) 
FROM tabla
WHERE condicion
---> Promedia los valores de una columna

```
## COUNT
Muestra la cantidad de valores de la columna
```SQL
SELECT COUNT(columna) 
FROM tabla 
WHERE condicion
---> Cuenta los registro de la tabla
SELECT COUNT(DISTINCT columna)
FROM tabla
WHERE condicion 
---> Muestra la cantdidad todos los valores diferentes

```
## HAVING
Filtra los grupos segun las condicones que coloquemos
```SQL
SELECT columna1 FROM tabla1 WHERE condicon 
GROUP BY columna1
HAVING concion
ORDER BY columna1
```
```SQL
SELECT columna1 FROM tabla1
GROUP BY columna1
HAVING COUNT = (condicion) 
```

[Regresar](Conceptos.md)