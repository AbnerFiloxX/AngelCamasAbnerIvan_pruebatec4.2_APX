#AngelCamasAbnerIvan_pruebaTec4.2_APX

📋 Descripción

Este proyecto es una prueba técnica para la gestión de clientes en una base de datos Oracle utilizando un contenedor ASO en Docker y ejecutado en IntelliJ. Se desarrolló utilizando JDBC generado por apx-cli.

🚀 Requisitos y Restricciones

La tabla debe estar en el esquema WIKJ con el nombre T_WIKJ_HAB_PRUEBAFINAL.

Campos de la tabla:

```id (Number(5), NOT NULL, PRIMARY KEY)

nuip (Number(10), único, no duplicado)

full_name (VARCHAR(50))

phone (VARCHAR(15))

address (VARCHAR(30))
```

Validación: No se permite insertar registros con nuip duplicado.

Seguridad: Se prohíbe SELECT * y consultas con ? para valores.

Salida esperada: Retorna la misma información insertada mediante un SELECT por id.
