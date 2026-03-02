# Gestor de Opiniones
API para la gestión de users, posts y feedback.
API para la gestión de usuarios, publicaciones y comentarios.
---

## Instalación y Ejecución

### 1️⃣ Instalar dependencias

```bash
npm install

```bash
npm run dev

Servidor por defecto
http://localhost:3005

Estado del Servidor
GET /opinionManager/v1/status

Base Url: users - usuarios
/opinionManager/v1/users

| Método | Endpoint   | Descripción      |
| ------ | ---------- | ---------------- |
| GET    | /users     | Listar usuarios  |
| POST   | /users     | Crear usuario    |
| PUT    | /users/:id | Editar usuario   |
| DELETE | /users/:id | Eliminar usuario |
