# Identity
## Propiedades

La propiedad Identity se puede establecer a uno o más campos de una tabla determinada.
Un campo con propiedad Identity activada, hará que su valor se incremente automáticamente a medida que se inserten registros en la tabla.
Es por ello que, para que un campo pueda ser Identity, su tipo de dato debe ser numérico.

>Por lo general establecemos Identity a un campo que es Primary Key. Con esto logramos que su valor no se duplique, generando registros únicos.

## Argumentos de la propiedad Identity
- Existe un argumento requerido llamado **Seed**.
- El argumento **Seed** define desde que valor comienza a incrementar su valor.
- Si el valor de **Seed** es 1, comenzará a incrementarse desde 1
Si el valor de **Seed** es 5, comenzará a incrementarse desde 5

También existe un argumento de la propiedad Identity, llamado **Increment**.
- Si el valor de **Increment** es 1, el valor del campo se guardará con valores correlativos *(Ejemplo: 1,2,3,4,5,6,7)*
- Si el valor de **Increment** es 2, el valor del campo se guardará con valores correlativos *(Ejemplo: 1,3,5,7,9,11,13)*

Para definir un campo con propiedad Identity (**Seed=1**, **Increment=2**) desde [Transact-SQL (T-SQL)](/Base-de-Datos/Transact-SQL.md):

```SQL
[NombreCampo] [int] IDENTITY(1,2)
```

Ejemplo de tabla con propiedad **IDENTITY**(1,2):

![](https://res.cloudinary.com/dtzgksveo/image/upload/v1687395562/PitooPlumo/SQL/Identity_a4rlkx.png "")

Ejemplo de tabla con propiedad **IDENTITY**(10,1):

![](https://res.cloudinary.com/dtzgksveo/image/upload/v1687395562/PitooPlumo/SQL/Identity2_eohsfj.png "")

## Activar Propiedad Identity
* Seleccionamos la tabla y damos clic derecho en la opción de **Design**

![](https://res.cloudinary.com/dtzgksveo/image/upload/v1688151878/PitooPlumo/SQL/Identity2_uthwa4.png)

* Mostrara las columna que contiene la tabla, en la parte inferior viene algunas opciones de la tabla 

* Nos dirigimos a la sección de **Identity Specification**

* En la opción de **(Is Identity)**, seleccionamos la opción de **YES**

![](https://res.cloudinary.com/dtzgksveo/image/upload/v1689624216/PitooPlumo/SQL/Identity4_mas68t.png)

[Regresar](./Elementos.md)