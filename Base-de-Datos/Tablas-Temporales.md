# Tablas Temporales
Las tablas temporales (también conocidas como tablas temporales con versión del sistema) son una característica de base de datos que ofrece soporte integrado para proporcionar información sobre los datos almacenados en la tabla en cualquier momento en el tiempo, en vez de únicamente los datos que son correctos en el momento actual determinado.

```SQL
CREATE TABLE #MiTablaTemporal (
    ID INT PRIMARY KEY,
    Nombre VARCHAR(50));
```

[Regresar](./Elementos.md)