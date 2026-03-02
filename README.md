# 🗂️ Gestor de Opiniones

🚀 TECNOLOGÍAS UTILIZADAS
🟢 Node.js
⚡ Express
🍃 MongoDB
🧩 Mongoose

📌 ¿Qué es el Gestor de Opiniones?
El Gestor de Opiniones es una API REST desarrollada para la gestión de:
👤 Usuarios
📝 Publicaciones (Posts)
💬 Comentarios (Feedback)
Permite realizar operaciones CRUD (Crear, Leer, Actualizar y Eliminar) sobre cada entidad, siguiendo buenas prácticas de arquitectura con controladores, modelos, rutas y middlewares.

## 📁 Estructura del Proyecto

```
GESTOROPINIONES/
│
├── configs/
├── fronted/
├── middlewares/
│   ├── check-validators.js
│   ├── handle-errors.js
│   └── request-limit.js
│
├── node_modules/
│
├── src/
│   ├── comments/
│   │   ├── comment.controller.js
│   │   ├── comment.model.js
│   │   └── comment.routes.js
│   │
│   ├── post/
│   │   ├── post.controller.js
│   │   ├── post.model.js
│   │   └── post.routes.js
│   │
│   └── user/
│       ├── user.controller.js
│       ├── user.model.js
│       └── user.routes.js
│
├── .env
├── .gitignore
├── index.js
├── LICENSE
├── OpinionesManager.postman_collection.json
├── package.json
├── package-lock.json
└── README.md
```
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


