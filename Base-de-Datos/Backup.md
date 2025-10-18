# Backup
Hace copia de seguridad de una base de datos completa de SQL Server para crear una copia de seguridad de la base de datos, o uno o más archivos o grupos de archivos de la base de datos para crear una copia de seguridad de archivo (BACKUP DATABASE). Además, con el modelo de recuperación completa o con el modelo de recuperación optimizado para cargas masivas de registros, realiza la copia de seguridad del registro de transacciones de la base de datos para crear una copia de seguridad de registros (BACKUP LOG).

1. **Full Backup (Copia de seguridad completa):**
* Contiene toda la información de la base de datos.
* Se realiza con la instrucción **BACKUP DATABASE**.
* Es el tipo más completo de backup y permite restaurar toda la base de datos. 
 
Ejemplo de comando T-SQL para realizar un backup completo:
```SQL
BACKUP DATABASE NombreDeTuBaseDeDatos 
TO DISK = 'Ruta\TuBackup.bak';
```

2. **Differential Backup (Copia de seguridad diferencial):**
* Contiene solo las modificaciones realizadas desde el último backup completo.
* Se realiza con la instrucción **BACKUP DATABASE ... WITH DIFFERENTIAL**.
* Permite reducir el tiempo de recuperación en comparación con realizar solo backups completos.

Ejemplo de comando T-SQL para realizar un backup diferencial:
```SQL
BACKUP DATABASE NombreDeTuBaseDeDatos 
TO DISK = 'Ruta\TuBackupDiferencial.bak' 
WITH DIFFERENTIAL;
```

3. **Transaction Log Backup (Copia de seguridad del registro de transacciones):**
* Contiene las transacciones realizadas desde el último backup de registro de transacciones.
* Se realiza con la instrucción **BACKUP LOG**.
* Es crucial para la recuperación puntual y la gestión de la recuperación en modo de recuperación completa.

Ejemplo de comando T-SQL para realizar un backup del registro de transacciones:

```SQL
BACKUP LOG NombreDeTuBaseDeDatos 
TO DISK = 'Ruta\TuBackupLog.trn';
```

[Regresar](./Elementos.md)