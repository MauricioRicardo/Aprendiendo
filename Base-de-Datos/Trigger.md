# Trigger
Crea un desencadenador DML, DDL o logon. Un desencadenador es un tipo especial de procedimiento almacenado que se ejecuta automáticamente cuando se produce un evento en el servidor de bases de datos. Los desencadenadores DML se ejecutan cuando un usuario intenta modificar datos mediante un evento de lenguaje de manipulación de datos (DML). Los eventos DML son instrucciones INSERT, UPDATE o DELETE de una tabla o vista. Estos desencadenadores se activan cuando se desencadena cualquier evento válido, con independencia de que las filas de la tabla se vean o no afectadas.

```SQL
CREATE TRIGGER tr_audit_changes
ON dbo.NombreTabla
AFTER UPDATE, INSERT, DELETE
AS
BEGIN
   -- Código para auditar cambios aquí
END;
```
[Regresar](Elementos.md)