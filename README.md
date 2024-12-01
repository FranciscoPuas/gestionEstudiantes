# Proyecto API Restful con Node.js, Express y Sequelize

Este proyecto es una API RESTful desarrollada con Node.js, Express y Sequelize, utilizando **PostgreSQL** como base de datos. La API gestiona recursos relacionados con estudiantes y se puede probar con herramientas como Postman.

---

## 🚀 **Tecnologías Utilizadas**
- **Node.js**: Entorno de ejecución para JavaScript en el servidor.
- **Express.js**: Framework para crear servidores HTTP y definir rutas.
- **Sequelize**: ORM para la interacción con la base de datos PostgreSQL.
- **dotenv**: Manejo de variables de entorno.
- **PostgreSQL**: Base de datos relacional.
- **Postman**: Herramienta para testear endpoints.

---

## 📂 **Estructura del Proyecto**
```plaintext
📁 proyecto
├── 📂 controllers        # Controladores para manejar solicitudes HTTP
├── 📂 models             # Modelos de Sequelize para la base de datos
├── 📂 routes             # Definición de rutas de la API
├── 📂 services           # Lógica de negocio y operaciones con la base de datos
├── 📄 server.js          # Configuración del servidor
├── 📄 .env               # Variables de entorno
├── 📄 README.md          # Documentación del proyecto
└── 📄 package.json       # Dependencias del proyecto
