# Funciones de Converción y Texto

## LEFT
Devuelve la parte izquierda de una cadena de caracteres con el número de caracteres especificado.
```SQL
SELECT LEFT(NomColumna, 5)   
FROM NomTabla
```

## RIGHT
Devuelve la parte derecha de una cadena de caracteres con el número de caracteres especificado.
```SQL
SELECT RIGHT(NomColumna, 5)   
FROM NomTabla
```

## LEN
Devuelve el número de caracteres de la expresión de cadena especificada, excluidos los espacios finales.
```SQL
SELECT LEN(NomColumna)   
FROM NomTabla
```

## LOWER
Devuelve una expresión de caracteres después de convertir en minúsculas los datos de caracteres en mayúsculas.
```SQL
SELECT LOWER(NomColumna)
FROM NomTabla
```

## UPPER
Devuelve una expresión de caracteres con datos de caracteres en minúsculas convertidos a mayúsculas.
```SQL
SELECT UPPER(NomColumna)
FROM NomTabla
```
## REPLACE
Reemplaza todas las instancias de un valor de cadena especificado por otro valor de cadena.
```SQL
SELECT REPLACE(NomColumna,'s','z')
FROM NomTabla
```

## REPLICATE
Repite un valor de cadena un número especificado de veces.
```SQL
SELECT REPLICATE(NomColumna, 2)
FROM NomTabla
```

## LTRIM
Quita el carácter de espacio u otros caracteres especificados del final de una cadena.
```SQL
SELECT LTRIM(NomColumna)
FROM NomTabla
```

## RTRIM
Quita el carácter de espacio u otros caracteres especificados del final de una cadena.
```SQL
SELECT RTRIM(NomColumna)
FROM NomTabla
```
## CONCAT
Esta función devuelve una cadena resultante de la concatenación, o la combinación, de dos o más valores de cadena de una manera integral.
```SQL
SELECT CONCAT(@Var1,@Var2,@Var3)
```

## GETDATE
Devuelve la marca de tiempo del sistema de base de datos actual como un valor datetime sin el desplazamiento de zona horaria de la base de datos. Este valor se deriva del sistema operativo del equipo donde la instancia de SQL Server se está ejecutando.
```SQL
SELECT GETDATE()
-->Fecha y hora actual
SELECT CONVERT (date, GETDATE())
-->Solo la fecha
SELECT CONVERT (time, GETDATE())
-->Solo la hora
```

## GETUTCDATE
Devuelve la marca de tiempo del sistema de la base de datos actual como un valor datetime. El ajuste de zona horaria de la base de datos no está incluido. Este valor representa la hora UTC actual (Hora universal coordinada). Este valor se deriva del sistema operativo del equipo donde la instancia de SQL Server se está ejecutando.
```SQL
SELECT GETUTCDATE()
```

## DATEADD
La parte de la fecha a la que DATEADD agrega un númeroentero. En esta tabla se enumeran todos los argumentos válidos de datepart.
```SQL
DATEADD(datepart, number, date)
```

## DATEDIFF
Esta función devuelve el recuento (como un valor entero con firma) de los límites datepart que se han cruzado entre los valores startdate y enddate especificados.
```SQL
DATEDIFF(datepart, startdate, enddate)
```

## DATEPART
Esta función devuelve un entero que representa el parámetro datepart especificado del parámetro date especificado.
```SQL
DATEPART(datepart , date)
```

## ISDATE
Devuelve 1 si expression es un valor válido de datetime; en caso contrario, devuelve 0.
```SQL
ISDATE(expression)
```

## CAST
Estas funciones convierten una expresión de un tipo de datos a otro.
```SQL
SELECT CAST(NomColumna AS date)
```

## CONVERT
Estas funciones convierten una expresión de un tipo de datos a otro.
```SQL
SELECT CONVERT(date, NomColumna)

SELECT CONVERT(date, Fecha, 112)
-->Le da formato diferente a las fechas, dependiendo el codigo del tercer valor
```
### Estilo de fecha y hora
Para una expression que tenga el tipo de datos de fecha u hora, style puede tener uno de los valores que se muestran en la siguiente tabla. Otros valores se procesan como 0.

|Sin el siglo (yy)<sup>1</sup>|Con el siglo (aaaa)|Estándar|Entrada/Salida<sup>(3)</sup>|
|:-:|:-:|-|-|
|- |0 o 100<sup>1,2</sup>|Valor predeterminado para **datetime** y **smalldatetime**|`mon dd yyyy hh:miAM` (o `PM`)
1|101|EE. UU.|1 = `mm/dd/yy` 101 = `mm/dd/yyyy`
2|102|ANSI|2 = `yy.mm.dd` 102 = `yyyy.mm.dd`
3|103|Británico/Francés| 3 = `dd/mm/yy` 103 = `dd/mm/yyyy`
4|104|Alemán|4 = `dd.mm.yy` 104 = `dd.mm.yyyy`
5|105|Italiano|5 = `dd-mm-yy` 105 = `dd-mm-yyyy`
6|106<sup>1</sup>|-|6 = `dd mon yy` 106 = `dd mon yyyy`
7|107|-|7 = `Mon dd, yy` 107 = `Mon dd, yyyy`
8 o 24|108|-|`hh:mi:ss`
|-|9 o 109<sup>1,2</sup>|Valor predeterminado + milisegundos|`mon dd yyyy` `hh:mi:ss:mmmAM` (o `PM`)
10|110|EE. UU.|10 = `mm-dd-aa` 110 = `mm-dd-yyyy`
11|111|Japón|11 = `aa/mm/dd` 111 = `yyyy/mm/dd`
12|112|ISO|12 = `aammdd` 112 = `yyyymmdd`
|-|13 o 113<sup>1,2</sup>|Europao predeterminado + milisegundos|`dd mon yyyy` `hh:mi:ss:mmm` (24 Horas)
14|114|-|`hh:mi:ss:mmm` (24 Horas)
|-|20 o 120<sup>2</sup>|ODBC canónico|`yyyy-mm-dd hh:mi:ss` (24 Horas)
|-|21 o 25 o 121<sup>2</sup>|ODBC canónico (con milisegundos), valor predeterminado para **time, date, datetime2 y datetimeoffset**|`yyyy-mm-dd` `hh:mi:ss.mmm` (24 Horas)
22|-|EE. UU.|`mm/dd/yy hh:mi:ssAM` (o `PM`)
|-|23|ISO8601|`yyyy-mm-dd`
|-|126<sup>4</sup>|ISO8601|`yyyy-mm-ddThh:mi:ss.mmm` (sin espacios)<sup>6</sup>
|-|127<sup>8,9</sup>|ISO8601 con zona horaria Z|`yyyy-MM-ddThh:mm:ss.fffZ` (sin espacios)<sup>6</sup>
|-|130<sup>1,2</sup>|Hijri<sup>5</sup>|`dd mon yyyy hh:mi:ss:mmmAM`<sup>7</sup>
|-|131<sup>2</sup>|Hijri<sup>5</sup>|`dd/mm/yyyy hh:mi:ss:mmmAM`

<sup>1</sup> Estos valores de estilo devuelven resultados no deterministas. Incluye todos los estilos (`yy`) (sin el siglo) y un subconjunto de estilos (`yyyy`) (con el siglo).

<sup>2</sup> Los valores predeterminados (**0 o 100, 9 o 109, 13 o 113, 20 o 120, 23 y 21 o 25 o 121**) siempre devuelven el siglo (`yyyy`).

<sup>3</sup> Entrada cuando se convierte en **datetime**; salida cuando se convierte en datos de caracteres.

<sup>4</sup> Diseñado para usarse con XML. Para convertir datos **datetime** o **smalldatetime** en datos de caracteres, consulte la tabla anterior para ver el formato de salida.

<sup>5</sup> Hijri es un sistema del calendario con varias variaciones. SQL Server utiliza el algoritmo kuwaití.

<sup>6</sup> En el caso de un valor 0 en milisegundos (`mmm`), el valor de fracción decimal en milisegundos no se mostrará. Por ejemplo, el valor `2022-11-07T18:26:20.000` se muestra como `2022-11-07T18:26:20`.

<sup>7</sup> En este estilo, `mon` es una representación Unicode Hijri multitoken del nombre completo del mes. Este valor no se representa correctamente en una instalación estadounidense predeterminada de SSMS.

<sup>8</sup> Solo se admite en la conversión de datos de caracteres a **datetime** o **smalldatetime**. Al convertir datos de caracteres que representan componentes de solo fecha o solo hora al tipo de datos **datetime** o **smalldatetime**, el componente de hora no especificado se establece en `00:00:00.000` y el componente de fecha no especificado se establece en `1900-01-01`.

<sup>9</sup> Use el indicador opcional de zona horaria `Z` para facilitar la asignación de valores XML de tipo **datetime** que contienen información de zona horaria a valores de tipo SQL Server **datetime** que no tienen zona horaria. `Z` indica la zona horaria en UTC-0. El desplazamiento `HH:MM`, en sentido `+` o `-`, indica otras zonas horarias. Por ejemplo: `2022-12-12T23:45:12-08:00`.

[Regresar](./Conceptos.md)