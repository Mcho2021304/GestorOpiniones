# 🗂️ Gestor de Opiniones

API REST para la gestión de **Usuarios**, **Publicaciones** y **Comentarios (Feedback)**.

---

# 🚀 Instalación y Ejecución

## 1️⃣ Instalar dependencias

```bash
npm install

npm run dev
```

http://localhost:3005

GET /opinionManager/v1/status

/opinionManager/v1/users

| Método | Endpoint   | Descripción      |
| ------ | ---------- | ---------------- |
| GET    | /users     | Listar usuarios  |
| POST   | /users     | Crear usuario    |
| PUT    | /users/:id | Editar usuario   |
| DELETE | /users/:id | Eliminar usuario |

{
  "name": "Sebastian",
  "username": "sebas123",
  "surname": "Cho",
  "email": "sebas@gmail.com",
  "password": "11111"
}

PUT /users/69a59951783f1f1083fb91ef
{
  "username": "juanEditado"
}

DELETE /users/69a59951783f1f1083fb91ef

/opinionManager/v1/posts

| Método | Endpoint   | Descripción          |
| ------ | ---------- | -------------------- |
| GET    | /posts     | Listar publicaciones |
| POST   | /posts     | Crear publicación    |
| PUT    | /posts/:id | Editar publicación   |
| DELETE | /posts/:id | Eliminar publicación |

{
  "title": "Mi primer post",
  "content": "Este es el contenido del post",
  "author": "69a59951783f1f1083fb91ef"
}

PUT /posts/69a59ad1783f1f1083fb91f3
{
  "content": "Contenido actualizado con PUT"
}

DELETE /posts/69a59ad1783f1f1083fb91f3

/opinionManager/v1/feedback
| Método | Endpoint      | Descripción         |
| ------ | ------------- | ------------------- |
| GET    | /feedback     | Listar comentarios  |
| POST   | /feedback     | Crear comentario    |
| PUT    | /feedback/:id | Editar comentario   |
| DELETE | /feedback/:id | Eliminar comentario |

{
  "text": "Este post está muy interesante",
  "userId": "69a59951783f1f1083fb91ef",
  "postId": "69a59ad1783f1f1083fb91f3"
}

PUT /feedback/69a59dab783f1f1083fb9200
{
  "text": "Comentario editado con PUT"
}

DELETE /feedback/69a59dab783f1f1083fb9200

📦 Tecnologías Utilizadas
Node.js
Express
MongoDB
Mongoose
