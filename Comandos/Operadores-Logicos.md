# Operadores Lógicos

## AND
Agregar mas de una condicion
```SQL
SELECT columna1
FROM tabla 
WHERE condicion AND condicion AND condicion
```
## OR
Para crear una condición mediante la combinación de dos expresiones booleanas
```SQL
SELECT columna1
FROM tabla
WHERE condicion OR condicion OR condicon
```
## IN
Seleccionar varios valores
```SQL
SELECT columna1
FROM tabla 
WHERE columna IN (valor1, valor2)

SELECT columna1 
FROM tabla 
WHERE columna NOT IN (valor1, valor2) 
---> Muestra los valores que no son iguales a la condicion
```
## LIKE
Muestra especificando 
```SQL
SELECT columna1, columna2, columna3
FROM tabla
WHERE columnaX LIKE 'patron'(% o _)

SELECT columna1
FROM tabla
WHERE columna1 NOT LIKE '%patron%'
---> Muestra los valores que no son iguales a la condicion
```
## NOT
No muestra lo de la condicion
```SQL
SELECT columna1
FROM tabla
WHERE NOT condicion
```
## BETWEEN
Selecciona valores dentro de un rango 
```SQL
SELECT columna1 
FROM tabla 
WHERE columna1 BETWEEN 'fecha' AND 'fecha' 

SELECT columna1 
FROM tabla 
WHERE columna1 NOT BETWEEN valor1 AND valor2 
---> Muestra valores fuera del rango 
```

[Regresar](Conceptos.md)