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

---
