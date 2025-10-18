## Funciones
Obtenga información sobre las categorías de las funciones integradas que se pueden usar con las bases de datos SQL. Puede usar las funciones integradas o crear las suyas propias.

## Funciones Escalares
Operan sobre un valor y después devuelven otro valor. Las funciones escalares se pueden utilizar donde la expresión sea válida.

```SQL
-- Definición de la función escalar
CREATE FUNCTION dbo.MultiplicarPorDos (@Numero INT)
RETURNS INT
AS
BEGIN
    DECLARE @Resultado INT
    SET @Resultado = @Numero * 2
    RETURN @Resultado
END;
```
## Funciones con valores de Tabla
Una función con valores de tabla es una función definida por el usuario que devuelve una tabla.

```SQL
CREATE FUNCTION dbo.ObtenerEmpleadosPorDepartamento(@DepartamentoID INT)
RETURNS TABLE
AS
RETURN (
    SELECT *
    FROM Empleados
    WHERE DepartamentoID = @DepartamentoID
);
```

[Regresar](Herramientas.md)