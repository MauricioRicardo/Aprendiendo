# Tipos de Datos

En SQL, un tipo de dato se refiere al formato del valor que puede almacenarse en un campo de una tabla. Los tipos de datos en SQL definen las características y las restricciones de los valores que pueden almacenarse en el mismo, como el rango de valores permitidos, el tamaño máximo o el formato.

## Descripción de Tipos de Datos
---
### **Numérico**
Nombre|Valor|Desde|Hasta
---|---|---|---|
BIT|1 Byte|0(False)|1(True)
TINYINT|1 Byte|0|255
SMALLINT|2 Byte|-32,768|32,767
INT| 4 Byte|-2,147,483,648 | 2,147,483,647
BIGINT|8 Bytes|-9,223,372,036,854,775,808|9,223,372,036,854,775,807
MONEY|8 Bytes|-922,337,203,685,477.5808|922,337,203,685,477.5807


Precisión|a|Escala|Valor
---:|---|---|---
1||9|5 Bytes
10||19|9 Bytes
20||28|13 Bytes
29||38|17 Bytes

---

### **Texto**
Nombre|Valor|Desde|Hasta
---|---|---|---|
CHAR|1 Byte por caracter|1 |8000
VARCHAR|1 Byte por caracter variable|1 |8000
NCHAR|2 Bytes por caracter|1 |4000
NVARCHAR|2 Bytes por caracter variable|1 |4000
BINARY|1 Byte por valor|1 |8000
VARBINARY|1 Byte por valor variable|1 |8000

---

## Fecha y Hora
Nombre|Valor|Formato|Desde|Hasta
---|---|---|---|---|
DATETIME| 8 Bytes|YYYY-MM-DD hh:mm:ss:nnn|01/01/1753|31/12/9999
DATE|3 Bytes|YYYY-MM-DD|01/01/0001|31/12/9999
TIME|5 Bytes|hh:mm:ss:nnnnnnn|00:00:00.0000000|23:59:59.9999999
SMALLDATETIME|4 Bytes|YYYY-MM-DD hh:mm:ss|01/01/1900 00:00:00|06/06/2079 23:59:59

---

## Repaso de Unidades de Medida en Informática
|Dato|Valor|
---:|----|
Bit| 0 ó 1
Byte(B)| 8 Bits
Kilobyte(Kb) | 1024 Bytes
Megabyte(MG)| 1024 Kilobytes
Gigabyte(GB)| 1024 Megabytes
Terabyte(TB)| 1024 Gigabytes
Petabyte(PB)| 1024 Terabytes
Exabyte(EB)| 1024 Petabyte

---

## Tipos de Datos Mas Utilizados
Tipo|Dato|
---|---|
Numérico|Enteros: INT, TINYINT, BIT
Numérico|Decimales: MONEY, DECIMAL
Texto| CHAR, VARCHAR
Fecha y Hora| DATETIME

---

[Para más información sobre los tipos de datos dar clic en este link](https://learn.microsoft.com/es-es/sql/t-sql/data-types/data-types-transact-sql?view=sql-server-ver16)

[Regresar](./Elementos.md)