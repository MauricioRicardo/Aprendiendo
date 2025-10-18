# Transacciones

Una transacción es una unidad única de trabajo. Si una transacción tiene éxito, todas las modificaciones de los datos realizadas durante la transacción se confirman y se convierten en una parte permanente de la base de datos. Si una transacción encuentra errores y debe cancelarse o revertirse, se borran todas las modificaciones de los datos.

SQL Server funciona en los modos de transacción siguientes:

Transacciones de confirmación automática
Cada instrucción individual es una transacción.

Transacciones explícitas
Cada transacción se inicia explícitamente con la instrucción BEGIN TRANSACTION y se termina explícitamente con una instrucción COMMIT o ROLLBACK.

Transacciones implícitas
Se inicia implícitamente una nueva transacción cuando se ha completado la anterior, pero cada transacción se completa explícitamente con una instrucción COMMIT o ROLLBACK.

Transacciones de ámbito de lote
Una transacción implícita o explícita de Transact-SQL que se inicia en una sesión de MARS (conjuntos de resultados activos múltiples), que solo es aplicable a MARS, se convierte en una transacción de ámbito de lote. Si no se confirma o revierte una transacción de ámbito de lote cuando se completa el lote, SQL Server la revierte automáticamente.

## BEGIN TRAN
Marca el punto de inicio de una transacción local explícita. Las transacciones explícitas empiezan con la instrucción BEGIN TRANSACTION y acaban con la instrucción COMMIT o ROLLBACK.
```SQL
-- Inicia la transacción
BEGIN TRAN

-- Realiza operaciones SQL
UPDATE Tabla SET Columna = Valor WHERE Condición

-- Verifica si todo está bien y confirma los cambios
COMMIT TRAN

-- O, en caso de error o decisión de revertir los cambios
ROLLBACK TRAN
```
## COMMIT TRAN
Marca el final de una transacción correcta, implícita o explícita. Si @@TRANCOUNT es 1, COMMIT TRANSACTION hace que todas las modificaciones de datos desde el inicio de la transacción sean parte permanente de la base de datos, libera los recursos de la transacción y reduce @@TRANCOUNT a 0. Si @@TRANCOUNT es mayor que 1, COMMIT TRANSACTION solo reduce @@TRANCOUNT en 1 y la transacción sigue activa.

```SQL
-- Inicia la transacción
BEGIN TRAN

-- Realiza operaciones SQL
UPDATE Tabla SET Columna = Valor WHERE Condición

-- Verifica si todo está bien y confirma los cambios
COMMIT TRAN
```

## ROLLBACK TRAN
Revierte una transacción explícita o implícita hasta el inicio de la transacción o hasta un punto de retorno dentro de la transacción. Puede usar ROLLBACK TRANSACTION para borrar todas las modificaciones de datos realizadas desde el inicio de la transacción o hasta un punto de retorno. También libera los recursos que mantiene la transacción.

No se incluyen los cambios realizados en variables locales o variables de tabla. No se borran con esta instrucción.
```SQL
-- Inicia la transacción
BEGIN TRAN

-- Realiza operaciones SQL
UPDATE Tabla SET Columna = Valor WHERE Condición

-- Algo sale mal o decides revertir los cambios
ROLLBACK TRAN

```

[Regresar](/Comandos/Conceptos.md)