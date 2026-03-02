# gestor_de_opiniones
Para clonar el proyecto en git bash


Para correr el proyecto en git bash
npm run dev

Para probar si esta funcionando
http://localhost:3005/opinionManager/v1/status 

User - Usuarios
http://localhost:3005/opinionManager/v1/users
Get - Lista 
Post - Crea
{
  "name": "Sebastian",
  "username": "sebas123",
  "surname": "cho",
  "email": "sebas@gmail.com",
  "password": "11111"
}

Put - Edita
http://localhost:3005/opinionManager/v1/users/69a59951783f1f1083fb91ef
{
  "username": "juanEditado"
}

Delete - Eliminar
http://localhost:3005/opinionManager/v1/users/69a59951783f1f1083fb91ef

Posts - Publicaciones
http://localhost:3005/opinionManager/v1/posts
Get- Lista
Post - Crea
se utiliza el id de un usuario al que va el post
{
  "title": "Mi primer post",
  "content": "Este es el contenido del post",
  "author": "69a59951783f1f1083fb91ef"
}

Put - Edita
http://localhost:3005/opinionManager/v1/posts/69a59ad1783f1f1083fb91f3
{
  "content": "Contenido actualizado con PUT"
}

Delete - Eliminar
http://localhost:3005/opinionManager/v1/posts/69a59951783f1f1083fb91ef

Feedback - Comentarios
http://localhost:3005/opinionManager/v1/feedback
Get - Lista
Post - Crea
Se utilizan id Reales de los usuarios y publicaciones creados anteriormente
{
  "text": "Este post está muy interesante",
  "userId": "69a59951783f1f1083fb91ef",
  "postId": "69a59ad1783f1f1083fb91f3"
}
Put - Edita
http://localhost:3005/opinionManager/v1/feedback/69a59dab783f1f1083fb9200
{
  "text": "Comentario editado con PUT"
}

Delete - Elminar
http://localhost:3005/opinionManager/v1/feedback/69a59951783f1f1083fb91ef
