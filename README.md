# Gestor de Opiniones
API para la gestión de users, posts y feedback.
---

## Instalación y Ejecución

### 1️⃣ Instalar dependencias

```bash
npm install

```bash
npm run dev

### 2️⃣ Instalar Ejecutar Servidor
Servidor por defecto
http://localhost:3005

### 3️⃣ Estado del Servidor
GET /opinionManager/v1/status

### 4️⃣ Servidor de Usuarios
/opinionManager/v1/users

| Método | Endpoint   | Descripción      |
| ------ | ---------- | ---------------- |
| GET    | /users     | Listar usuarios  |
| POST   | /users     | Crear usuario    |
| PUT    | /users/:id | Editar usuario   |
| DELETE | /users/:id | Eliminar usuario |

📝Crear un Usuario
{
  "name": "Sebastian",
  "username": "sebas123",
  "surname": "cho",
  "email": "sebas@gmail.com",
  "password": "11111"
}

📝Editar Usuario
PUT /users/69a59951783f1f1083fb91ef
{
  "username": "juanEditado"
}

📝Eliminar Usuario
DELETE /users/69a59951783f1f1083fb91ef

### 5️⃣ Servidor de Publicaciones
/opinionManager/v1/posts

| Método | Endpoint   | Descripción          |
| ------ | ---------- | -------------------- |
| GET    | /posts     | Listar publicaciones |
| POST   | /posts     | Crear publicación    |
| PUT    | /posts/:id | Editar publicación   |
| DELETE | /posts/:id | Eliminar publicación |

📝Crear una Publicacion
{
  "title": "Mi primer post",
  "content": "Este es el contenido del post",
  "author": "69a59951783f1f1083fb91ef"
}

📝Editar Publicacion
PUT /posts/69a59ad1783f1f1083fb91f3
{
  "content": "Contenido actualizado con PUT"
}

📝Eliminar Publicacion
DELETE /users/69a59951783f1f1083fb91ef

### 6️⃣ Servidor de Comentarios
/opinionManager/v1/feedback

| Método | Endpoint      | Descripción         |
| ------ | ------------- | ------------------- |
| GET    | /feedback     | Listar comentarios  |
| POST   | /feedback     | Crear comentario    |
| PUT    | /feedback/:id | Editar comentario   |
| DELETE | /feedback/:id | Eliminar comentario |

📝Crear un Comentario
{
  "text": "Este post está muy interesante",
  "userId": "69a59951783f1f1083fb91ef",
  "postId": "69a59ad1783f1f1083fb91f3"
}

📝Editar Comentario
PUT /feedback/69a59dab783f1f1083fb9200
{
  "text": "Comentario editado con PUT"
}

📝Eliminar Comentario
DELETE /feedback/69a59dab783f1f1083fb9200
