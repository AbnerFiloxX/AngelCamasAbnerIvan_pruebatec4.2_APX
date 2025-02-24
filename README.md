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
🛠️ Tecnologías utilizadas

Java con JDBC

Oracle Database

Docker (ASO Container)

IntelliJ IDEA

Postman para pruebas
JSON ingresado para prueba
```{
  "dtoIn": {
    "id": "26",
    "nuip": "12345",
    "full_name": "Abnercito Camas",
    "phone": "9842805504",
    "address": "Calle San Roque #7"
  }
}
```
se esperaba que tuviera un retorno de la informacion y se guardara en la base de datos pero no fue así,salia el error siguiente
```{
    "messages": [
        {
            "code": "01211000",
            "message": "SE HA PRODUCIDO EL ERROR QWPO01211005 DURANTE EL PROCESAMIENTO DE LA TRANSACCION",
            "adviceUuaa": "QWPO",
            "type": "ERROR"
        }
    ]
}
```
#me arriesgaré a culpar al entorno de apx 
