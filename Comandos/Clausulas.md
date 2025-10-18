# Cláusulas

## TOP
Se utiliza en SQL Server para limitar el número de filas devueltas por una consulta. Puedes usarlo en combinación con la cláusula **SELECT** para obtener un número específico de filas o un porcentaje de las filas resultantes.
```SQL
SELECT TOP(numero) columna 
FROM tabla 
WHERE condicion
```

## ORDER BY
 Se utiliza para ordenar el resultado de una consulta según una o más columnas específicas, ya sea en orden ascendente (**ASC**) o descendente (**DESC**).
```SQL
SELECT columnas
FROM nombre_tabla
ORDER BY columna1 [ASC | DESC], columna2 [ASC | DESC]
```

## DISTINCT
Se utiliza en una consulta **SELECT** para devolver solamente valores únicos en una columna específica. Esto significa que si tienes duplicados en esa columna, solo se mostrará un valor único de cada conjunto de duplicados.
```SQL
SELECT DISTINCT columna
FROM nombre_tabla;
```

## GROUP BY
Se utiliza para agrupar filas que tienen valores iguales en una o más columnas específicas. Luego, puedes aplicar funciones de agregación, como **SUM, AVG, COUNT, MAX o MIN**, a cada grupo resultante. Esto es útil cuando quieres realizar operaciones sobre conjuntos de datos agrupados.
```SQL
SELECT columna1, columna2
FROM nombre_tabla
GROUP BY columna1, columna2;
```

## WHERE
Se utiliza para filtrar filas de un conjunto de resultados basándose en una condición especificada. Esta cláusula se utiliza generalmente en combinación con la cláusula **SELECT**, pero también puede usarse con otras cláusulas como **UPDATE, DELETE o SELECT INTO**.
```SQL
SELECT columnas
FROM nombre_tabla
WHERE condicion;
```

[Regresar](./Conceptos.md)