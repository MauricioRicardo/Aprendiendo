# SubConsultas
Sub consulta con alias
```SQL
SELECT Apellido, Nombre, IDPais, Observacion,
	(SELECT Ps.pais FROM Pais Ps WHERE Ps.idPais = Pa.idPais) AS DescPais
FROM Paciente Pa
WHERE idPaciente =1
```

[Regresar](Elementos.md)