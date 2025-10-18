# Normalización de Base de Datos

### Tabla Paciente (Sin Normalizar)
![Tabla sin Normalizar](https://res.cloudinary.com/dtzgksveo/image/upload/v1687807242/PitooPlumo/SQL/Normalizar_p0lfhx.png "Tabla sin Normalizar")

## Primera Forma de Normalización
Se dice que una tabla está en *Primera Forma Normal* si y sólo si todos sus **Campos (Atributos)** contienen valores atómicos. Esto quiere decir que cada **Atributo de la Tabla** deberá tener un único valor para una ocurrencia de la **Entidad**. No se permitirán grupos repetitivos.

### Tabla Paciente con Primera Forma de Normalizar
![Primera Forma de Normalizar](https://res.cloudinary.com/dtzgksveo/image/upload/v1687807242/PitooPlumo/SQL/Normalizar1_usovfd.png "Primera Forma de Normalizar")

## Segunda Forma de Normalización
Una tabla está en *Segunda Forma Normal* si y sólo si está en **Primera Forma Normal** y todos los **Atributos no Clave** dependen por completo de la **Llave primaria**.

## Tercera Forma de Normalización
Una tabla está en **Tercera Forma Normal** si y sólo si está en *Segunda Forma Normal* y los **Atributos no Clave** son independientes entre sí. Esto quiere decir que los valores de los **Atributos** dependen sólo de la **Llave Primaria** y no dependen de otro **Atributo no Clave**. El valor del **Atributo** no debe depender del valor de otro **Atributo no clave**.

### Tabla Paciente con Segunda y Tercera Forma de Normalización
![Segunda y Tercera Forma de Normalización](https://res.cloudinary.com/dtzgksveo/image/upload/v1687807242/PitooPlumo/SQL/Normalizar2y3_fkzojg.png "Segunda y Tercera Forma de Normalización")

### Tabla Pais
![Tabla Pais](https://res.cloudinary.com/dtzgksveo/image/upload/v1687807242/PitooPlumo/SQL/TablaPais_yimrbq.png "Tabla Pais")

### Tabla Medico
![Tabla Medico](https://res.cloudinary.com/dtzgksveo/image/upload/v1687807242/PitooPlumo/SQL/TablaMedico_qluewm.png "Tabla Medico")

### Tabla Turno Paciente
![Tabla Turno Paciente](https://res.cloudinary.com/dtzgksveo/image/upload/v1687807242/PitooPlumo/SQL/TablaTurnoPaciente_pxpnun.png "Tabla Tunor Paciente")

[Mas información sobre la Normalización de la Base de Datos ingresa a este link](https://learn.microsoft.com/es-es/office/troubleshoot/access/database-normalization-description)

[Regresar](./Elementos.md)