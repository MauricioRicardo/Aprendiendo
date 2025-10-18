# Stored Procedure

Un procedimiento almacenado de SQL Server es un grupo de una o varias instrucciones Transact-SQL o una referencia a un método de Common Runtime Language (CLR) de Microsoft .NET Framework. Los procedimientos se asemejan a las construcciones de otros lenguajes de programación, porque pueden:

* Aceptar parámetros de entrada y devolver varios valores en forma de parámetros de salida al programa que realiza la llamada.

* Contener instrucciones de programación que realicen operaciones en la base de datos. Entre otras, pueden contener llamadas a otros procedimientos.

* Devolver un valor de estado a un programa que realiza una llamada para indicar si la operación se ha realizado correctamente o se han producido errores, y el motivo de estos.


## Crear Stored Procedure
```SQL
CREATE PROC nombre (@variable INT)
AS
SELECT * FROM tabla WHERE columna = @variable
GO
```

```SQL
SET ANSI_NULLS ON
GO
---> No muestre datos NULL
SET QUOTED_IDENTIFIER ON
GO
---> Se pueden crear objetos con palabra reservadas
```

## Modificar Stored Procedure
```SQL
ALTER PROC nombre (@variable INT)
AS
SELECT * FROM tabla WHERE columna = @variable
GO
```

## Ejecutar Stored Procedure
```SQL
EXEC nombre VALOR
```

[Para mas información en este link](https://learn.microsoft.com/es-es/sql/relational-databases/stored-procedures/stored-procedures-database-engine?view=sql-server-ver16)

[Regresar](Herramientas.md)