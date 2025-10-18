# Variables

Declara variable
```sql
DECLARE @nombrevariable CHAR(1) = 'A'
```

En caso de que la variable sea NULL muestre otro dato
```sql
DECLARE @nombrevariable1 CHAR(1)
DECLARE @nombrevariable2 CHAR(1)
SET @nombrevariable1 = ISNULL (@nombrevariable2, 'A')
```
[Regresar](./Elementos.md)