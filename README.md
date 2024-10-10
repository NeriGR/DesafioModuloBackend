# Desafío Backend

Proyecto basado en la funcionalidad de dev.to, utilizado para crear, modificar, regitrar POSTS en la red social.


## Teconologias y herramientas

Node.js
Express
MongoDB
bcryptjs
dotenv
http-errors
mongoose
JWT
clean architecture

## Se utilizaron las entidades:
## User

Atributos:

- name (string)
- profilePic (string)
- email (string)
- password (string)
- created_at (date)
- updated_at (date)

### POST /user

Para permitir el registro a los nuevos usuarios

No requiere autorización

### GET /user/:id

Para obtener la información de un usuario por id

No requiere autorización

---

### POST /auth/login

Para otorgar un nuevo JWT cada que es llamado

No requiere autorización

## Post

Atributos:

- title (string)
- image (string)
- body (string )
- user (ObjectId referencia a UserId)
- created_at (date)
- updated_at (date)

### POST /posts

Para crear un nuevo post, el post creado será asignado al usuario que llamó este endpoint

Requiere autorización

### GET /posts

Para listar todos los posts

- Debe soportar el filtrado por titulo usando un query param llamado `search`

No requiere autorización

### PATCH /posts/:id

Para permitir actualizar un post

- No se debe permitir cambiar el usuario de un post

Requiere autorización

### DELETE /posts/:id

Para permitir borrar un post

- Solo el usuario que creo el post debe ser capaz de ejecutar esta acción

#### Crear una API utilizando MongoDB, Express, y Mongoose es una buena práctica porque ofrece un desarrollo rápido, eficiente y escalable. MongoDB, al ser una base de datos NoSQL, permite manejar grandes volúmenes de datos no estructurados con flexibilidad. Express simplifica la creación de servidores y APIs RESTful en Node.js, mientras que Mongoose facilita la interacción con MongoDB mediante un esquema estructurado y validación robusta. Juntos, estos componentes forman una arquitectura moderna, ágil y apta para proyectos de diferentes escalas.

Aprovecho este espacio para agradecer sinceramente que hayan recibido el trabajo a pesar de la demora. Su comprensión es muy valorada. ¡Gracias!





