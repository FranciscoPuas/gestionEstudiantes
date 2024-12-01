Proyecto API RESTful con Node.js, Express y Sequelize
Este proyecto es una API RESTful desarrollada con Node.js, Express y Sequelize, utilizando PostgreSQL como base de datos. La API gestiona recursos relacionados con estudiantes y se puede probar con herramientas como Postman.
🚀 Tecnologías Utilizadas

Node.js: Entorno de ejecución para JavaScript en el servidor.
Express.js: Framework para crear servidores HTTP y definir rutas.
Sequelize: ORM para la interacción con la base de datos PostgreSQL.
dotenv: Manejo de variables de entorno.
PostgreSQL: Base de datos relacional.
Postman: Herramienta para testear endpoints.

📂 Estructura del Proyecto
Copy📁 proyecto
├── 📂 controllers        # Controladores para manejar solicitudes HTTP
├── 📂 models             # Modelos de Sequelize para la base de datos
├── 📂 routes             # Definición de rutas de la API
├── 📂 services           # Lógica de negocio y operaciones con la base de datos
├── 📄 server.js          # Configuración del servidor
├── 📄 .env               # Variables de entorno
├── 📄 README.md          # Documentación del proyecto
└── 📄 package.json       # Dependencias del proyecto


##📋 Rutas para Testeo en Postman
Estudiantes
MétodoEndpointDescripciónEjemplo de Cuerpo (JSON)GET/api/estudiantesObtener todos los estudiantes.N/AGET/api/estudiantes/:idObtener un estudiante por ID.N/APOST/api/estudiantesCrear un nuevo estudiante.Ver ejemplo abajoPUT/api/estudiantesActualizar un estudiante.Ver ejemplo abajoDELETE/api/estudiantes/:idEliminar un estudiante por ID.N/A
Ejemplo de Cuerpo para Crear un Estudiante (POST /api/estudiantes)
jsonCopy{
    "idEstudiante": 1,
    "rutEstudiante": "12345678-9",
    "nombreEstudiante": "Juan Pérez",
    "fechaNacimiento": "2000-01-01",
    "direccion": "Calle Falsa 123",
    "correo": "juan.perez@example.com",
    "telefono": "987654321"
}
Ejemplo de Cuerpo para Actualizar un Estudiante (PUT /api/estudiantes)
jsonCopy{
    "idEstudiante": 1,
    "rutEstudiante": "12345678-9",
    "nombreEstudiante": "Juan Pérez Actualizado",
    "fechaNacimiento": "2000-01-01",
    "direccion": "Calle Actualizada 456",
    "correo": "juan.perez.nuevo@example.com",
    "telefono": "123456789"
}
Ejemplo de Respuesta Exitosa
GET /api/estudiantes
jsonCopy{
    "msg": "Los estudiantes son:",
    "datos": [
        {
            "idEstudiante": 1,
            "rutEstudiante": "12345678-9",
            "nombreEstudiante": "Juan Pérez",
            "fechaNacimiento": "2000-01-01",
            "direccion": "Calle Falsa 123",
            "correo": "juan.perez@example.com",
            "telefono": "987654321"
        }
    ]
}
POST /api/estudiantes
jsonCopy{
    "msg": "El usuario con rut 12345678-9 se insertó correctamente",
    "datos": {
        "idEstudiante": 1,
        "rutEstudiante": "12345678-9",
        "nombreEstudiante": "Juan Pérez",
        "fechaNacimiento": "2000-01-01",
        "direccion": "Calle Falsa 123",
        "correo": "juan.perez@example.com",
        "telefono": "987654321"
    }
}
🛠️ Pruebas con Postman

Abre Postman e importa los endpoints.
Configura las solicitudes como se indica en las tablas anteriores.
Asegúrate de que el servidor está corriendo en http://localhost:3000 antes de probar.
Realiza pruebas CRUD para verificar el funcionamiento de la API.

📝 Licencia
Este proyecto está bajo la licencia MIT.
