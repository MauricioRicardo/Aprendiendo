# Estructuras de Control
Para evaluar un bloque de codigo
## IF
Impone condiciones en la ejecución de una instrucción Transact-SQL. La instrucción Transact-SQL que sigue a una palabra clave IF y a su condición se ejecuta si la condición se cumple: la expresión booleana devuelve TRUE. La palabra clave opcional ELSE introduce otra instrucción Transact-SQL que se ejecuta cuando la condición IF no se cumple: la expresión booleana devuelve FALSE.

```SQL
IF Variable
    Condicion
ELSE
    Condicion
```

## BEGIN END
Incluye una serie de instrucciones Transact-SQL de forma que se pueda ejecutar un grupo de instrucciones Transact-SQL. BEGIN y END son palabras clave del lenguaje de control de flujo.

```SQL
IF Variable
BEGIN
    Bloque de instrucciones
END
ELSE
BEGIN
    Bloque de instrucciones
END
```

## EXISTS
Especifica una subconsulta para probar la existencia de filas.
 ```SQL
SELECT columna1
FROM tabla1
WHERE EXISTS (SELECT columna1 FROM tabla WHERE condicion)
 ```

## WHILE
Establece una condición para la ejecución repetida de una instrucción o bloque de instrucciones SQL. Las instrucciones se ejecutan repetidamente siempre que la condición especificada sea verdadera. Se puede controlar la ejecución de instrucciones en el bucle WHILE con las palabras clave BREAK y CONTINUE.
```SQL
DECLARE @Contador INT = 0

WHILE @Contador <= 10
BEGIN
	PRINT @Contador
	SET @Contador = @Contador + 1
END
```
## CASE
Evalúa una lista de condiciones y devuelve una de las varias expresiones de resultado posibles.

La expresión CASE tiene dos formatos:

 - La expresión CASE sencilla compara una expresión con un conjunto de expresiones sencillas para determinar el resultado.

 - La expresión CASE buscada evalúa un conjunto de expresiones booleanas para determinar el resultado.

Ambos formatos admiten un argumento ELSE opcional.

```SQL
DECLARE @Valor INT
DECLARE @Resultado VARCHAR(10) = ' '
SET @Valor = 0

SET @Resultado = (CASE WHEN @Valor = 10 THEN 'ROJO'
						WHEN @Valor = 20 THEN 'VERDE'
						WHEN @Valor = 30 THEN 'AZUL'
					ELSE 'GRIS'
				END)
PRINT @Resultado
```

```SQL
SELECT *,(CASE WHEN estado = 0 THEN 'VERDE'
				WHEN estado = 1 THEN 'ROJO'
				WHEN estado = 2 THEN 'AZUL' 
			ELSE 'GRIS'
		END)
FROM Turno
```

## RETURN
Sale incondicionalmente de una consulta o procedimiento. RETURN es inmediata y completa, y se puede utilizar en cualquier punto para salir de un procedimiento, lote o bloque de instrucciones. Las instrucciones que siguen a RETURN no se ejecutan
```SQL
DECLARE @Contador INT = 0

WHILE @Contador <= 10
BEGIN
	PRINT @Contador
	SET @Contador = @Contador + 1
	IF @Contador = 3
		RETURN
		PRINT 'Hola'
END
```

## BREAK
BREAK sale del bucle WHILE actual. Si el bucle WHILE actual está anidado dentro de otro, BREAK solo sale del bucle actual y se proporciona el control a la siguiente instrucción del bucle exterior.

BREAK suele encontrarse dentro de una instrucción IF.

```SQL
DECLARE @Contador INT = 0

WHILE @Contador <= 10
BEGIN
	PRINT @Contador
	SET @Contador = @Contador + 1
		IF @Contador = 3
		BREAK
END
PRINT 'Hola'
```

## TRY CATCH
Implementa un mecanismo de control de errores para Transact-SQL. Se puede incluir un grupo de instrucciones Transact-SQL en un bloque TRY. Si se produce un error en el bloque TRY, el control se suele transferir a otro grupo de instrucciones que está incluido en un bloque CATCH.

```SQL
BEGIN TRY
	SET @Contador = 'Texto'
END TRY

BEGIN CATCH
	PRINT 'No es posbible asignar un texto a la variable contador'
END CATCH
```

[Regresar](Conceptos.md)