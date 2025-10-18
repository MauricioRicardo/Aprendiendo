# Relaciones Entre Tablas

## Relacion de Uno a Uno

En una relación de uno a uno, un registro de una tabla se asocia a uno y solo un registro de otra tabla. Por ejemplo, en una base de datos de un centro educativo, cada alumno tiene solamente un ID de estudiante, y cada ID de estudiante se asigna solo a una persona.

Una relación de uno a uno se represente de la siguiente manera:

![](https://res.cloudinary.com/dtzgksveo/image/upload/v1689792877/PitooPlumo/SQL/RelacionTablas_zaadgz.png)

En este ejemplo, el campo de clave de cada tabla, ID de estudiante, se ha diseñado para contener valores exclusivos. En la tabla Alumnos, el campo ID de estudiante es la clave principal; en la tabla Información de contacto, el campo ID de estudiante es una clave externa.

Esta relación devuelve registros relacionados cuando el valor del campo ID de estudiante de la tabla Información de contacto es el mismo que el del campo ID de estudiante de la tabla Alumnos.

![](https://res.cloudinary.com/dtzgksveo/image/upload/v1689792877/PitooPlumo/SQL/RelacionTablas1_dmvrs0.png)

## Relacion de Uno a Muchos
En una relación de uno a muchos, un registro de una tabla se puede asociar a uno o varios registros de otra tabla.. Por ejemplo, cada cliente puede tener varios pedidos de ventas.

Una relación de uno a muchos se represente de la siguiente manera:

![](https://res.cloudinary.com/dtzgksveo/image/upload/v1689792877/PitooPlumo/SQL/RelacionTablas2_xl3s06.png)

En este ejemplo, el campo de clave principal de la tabla Clientes, ID de cliente, se ha diseñado para contener valores exclusivos. El campo de clave externa de la tabla Pedidos, ID de cliente, se ha diseñado para permitir varias instancias del mismo valor.

Esta relación devuelve registros relacionados cuando el valor del campo ID de cliente de la tabla Pedidos es el mismo que el valor del campo ID de cliente de la tabla Clientes.

![](https://res.cloudinary.com/dtzgksveo/image/upload/v1689792877/PitooPlumo/SQL/RelacionTablas3_mas9a8.png)

Como las relaciones son bidireccionales, también hay relaciones de muchos a uno.

## Relacion de Muchos a Muchos
Una relación de muchos a muchos se produce cuando varios registros de una tabla se asocian a varios registros de otra tabla. Por ejemplo, existe una relación de muchos a muchos entre los clientes y los productos: los clientes pueden comprar varios productos y los productos pueden ser comprados por muchos clientes.

Por lo general, los sistemas de bases de datos relacionales no permiten implementar una relación directa de muchos a muchos entre dos tablas. Tenga en cuenta el ejemplo de seguimiento de facturas. Si había muchas facturas con el mismo número de factura y uno de sus clientes preguntó acerca de ese número de factura, no sabría a qué número se refería. Este es el motivo por el que se debe asignar un valor exclusivo a cada factura.

Para evitar este problema, puede dividir la relación de muchos a muchos en dos relaciones de uno a muchos mediante el uso de una tercera tabla denominada tabla de unión. Cada registro de una tabla de unión incluye un campo de coincidencia que contiene el valor de las claves principales de las dos tablas que se unen. (En la tabla de unión, estos campos de coincidencia son claves externas). Estos campos de clave externa se rellenan con datos, ya que los registros de la tabla de unión se crean desde cualquiera de las tablas que se unen.

Un ejemplo típico de una relación de muchos a muchos es aquella entre los estudiantes y las clases. Un estudiante puede matricularse en muchas clases y una clase puede incluir muchos estudiantes.

En el siguiente ejemplo, se incluye una tabla Alumnos, que contiene un registro para cada estudiante, y una tabla Clases, que contiene un registro para cada clase. Una tabla de unión, Matrículas, crea una relación de uno a muchos, una entre cada una de las dos tablas.

![](https://res.cloudinary.com/dtzgksveo/image/upload/v1689792877/PitooPlumo/SQL/RelacionTablas4_k6fo7s.png)

La clave principal ID de estudiante identifica de forma exclusiva a cada estudiante de la tabla Alumnos. La clave principal ID de clase identifica de forma exclusiva cada clase de la tabla Clases. La tabla Matrículas contiene las claves externas ID de estudiante e ID de clase.

**Para configurar una tabla de unión para una relación de muchos a muchos:**

1. Mediante el uso del ejemplo, anterior, cree una tabla denominada Matrículas. Esta será la tabla de unión.

2. En la tabla Matrículas, cree un campo ID de estudiante y un campo ID de clase.

    Por lo general, las tablas de unión contienen campos que no tienen sentido en otras tablas. Puede añadir campos a la tabla Matrículas, como un campo Fecha para mantener un registro de cuándo alguien inició una clase y un campo Coste para rastrear cuánto pagó un estudiante por realizar una clase.
3.  Cree una relación entre los dos campos ID de estudiante de las tablas. A continuación, cree una relación entre los dos campos ID de clase de las tablas.  

### Nota

* Mediante este diseño, si un estudiante se matricula en tres clases, ese estudiante tendrá un registro en la tabla Alumnos y tres registros en la tabla Matrículas: un registro para cada clase en la que se ha matriculado el estudiante.

---
Las relaciones entre tablas no son obligatorias. Una base de datos puede no tener tablas relacionadas.

No obstante, una BD sin relaciones, corre el riesgo de perder la integridad de los datos en las tablas, ya que no tiene definidas las Reglas de Integridad Referencial.

**¿Qué son éstas Reglas?**

Son propiamente las relaciones entre tablas, en las que un campo Primary Key (PK) se relaciona un campo de otra tabla (del mismo tipo de dato), al cuál llamamos Foreign Key (FK).

**¿De que me sirve crear esta relación?**

Esta relación NO permitirá colocar un valor en el campo definido como FK, que no esté definido en la tabla definida con el campo PK.

**Veamos este ejemplo:**

Tabla Paciente (campo idpais FK)

Tabla Pais (campo idpais PK)

 * Si tratamos de insertar un Paciente nuevo con un código de país que no existe en la tabla país, devolverá error y no permitirá su grabación.

**¿Porqué no me permite insertar el registro?**

* Porque se ha definido la relación entre ambas tablas. Es una Regla de Integridad Referencial, y previene que guardemos registros con valores indefinidos.

* Esto hace que del lado de la interfaz de usuario, siempre se pueda visualizar información consistente.

**¿Qué sucede si quiero eliminar un registro de la tabla Pais, cuyo país está asignado a un Paciente?**

* Al igual que antes, la Regla de Integridad no nos permitirá eliminar el país, hasta que cambiemos el país del Paciente por otro.

* Esta es la característica principal de las Bases de Datos Relacionales.

[Para mas informacion dar clic en link](https://fmhelp.filemaker.com/help/18/fmp/es/index.html#page/FMP_Help%2Frelated-tables-files.html%23)

[Regresar](./Elementos.md)