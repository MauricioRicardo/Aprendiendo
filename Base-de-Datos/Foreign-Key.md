# Foreign Key (FK)

- La *Foreign Key* o su traducción *Llave Foránea*, debe ser del mismo tipo del dato que su campo relacionado.
- El valor del campo definido como *Foreign Key* puede ser NULL.
Una tabla puede tener más de un campo *Foreign Key*.

![Imagen no disponible por el momento](https://res.cloudinary.com/dtzgksveo/image/upload/v1687375362/PitooPlumo/SQL/Foreign_Key_xhjhcv.png "Ejemoplo de una Foreign Key") 

Una *Foreign Key*, es aquella relación entre la **Primary Key** de una Tabla
llamémosle A, la cuál está relacionada directamente con uno o más campos del mismo tipo en una
Tabla B.

La Tabla B solo podrá tener valores en el campo con *Foreign Key*, que existan únicamente en la Tabla
A. No podrá tener otros valores.

La *Foreign Key* también es una de las reglas de **Integridad Referencial de Base de Datos**.

[Regresar](./Elementos.md)