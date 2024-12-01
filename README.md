Este proyecto es una API RESTful desarrollada con **Node.js**, **Express** y **Sequelize**, utilizando **PostgreSQL** como base de datos. La API gestiona recursos relacionados con estudiantes y se puede probar con herramientas como **Postman**.

## 🚀 Tecnologías Utilizadas

- **Node.js**: Entorno de ejecución para JavaScript en el servidor.
- **Express.js**: Framework para crear servidores HTTP y definir rutas.
- **Sequelize**: ORM para la interacción con la base de datos PostgreSQL.
- **dotenv**: Manejo de variables de entorno.
- **PostgreSQL**: Base de datos relacional.
- **Postman**: Herramienta para testear endpoints.
## 📋 Rutas para Testeo en Postman

### **Estudiantes**

| **Método** | **Endpoint**             | **Descripción**                  | **Ejemplo de Cuerpo (JSON)** |
|------------|---------------------------|-----------------------------------|------------------------------|
| GET        | `/api/estudiantes`        | Obtener todos los estudiantes.    | N/A                          |
| GET        | `/api/estudiantes/:id`    | Obtener un estudiante por ID.     | N/A                          |
| POST       | `/api/estudiantes`        | Crear un nuevo estudiante.        | Ver ejemplo abajo            |
| PUT        | `/api/estudiantes`        | Actualizar un estudiante.         | Ver ejemplo abajo            |
| DELETE     | `/api/estudiantes/:id`    | Eliminar un estudiante por ID.    | N/A                          |


### Ejemplo de Cuerpo para Crear un Estudiante (POST `/api/estudiantes`)

```json
{
    "idEstudiante": 1,
    "rutEstudiante": "12345678-9",
    "nombreEstudiante": "Juan Pérez",
    "fechaNacimiento": "2000-01-01",
    "direccion": "Calle Falsa 123",
    "correo": "juan.perez@example.com",
    "telefono": "987654321"
}
Ejemplo de Cuerpo para Actualizar un Estudiante (PUT /api/estudiantes)
json
Copiar código
{
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
json
Copiar código
{
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
json
Copiar código
{
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
