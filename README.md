# UnaHur Anti-Social Net - API BackEnd

Este proyecto es una versión mínima de la API necesaria para el Trabajo Práctico de la materia FrontEnd (React). Permite trabajar con publicaciones, usuarios, comentarios y etiquetas.

> 📦 Este backend está pensado como una “caja negra” para que los estudiantes puedan consumirlo desde React sin necesidad de modificar el código.

---

## 🚀 Requisitos

- Node.js instalado (versión recomendada: 16 o superior)
- Git (opcional, si se descarga desde un repositorio)

---

## 📂 Instalación

1. Descargar y descomprimir el archivo `backend-api.zip`.
2. Abrir una terminal dentro de la carpeta `backend-api`.
3. Instalar las dependencias:

```bash
npm install
```

4. Crear y poblar la base de datos con datos de ejemplo:

```bash
node seed.js
```

5. Iniciar el servidor:

```bash
npm start
```

---

## 🌐 API disponible

Una vez iniciado, el servidor quedará disponible por defecto en:

```
http://localhost:3001
```

---

## 🔁 Endpoints disponibles

### Usuarios
- `GET /users`: devuelve todos los usuarios
- `GET /users/:id`: devuelve un usuario por ID
- `POST /users`: crea un nuevo usuario (con `nickName` y `email`)

### Publicaciones
- `GET /posts`: lista todas las publicaciones
- `GET /posts/:id`: detalle de una publicación
- `POST /posts`: crear nueva publicación

### Comentarios
- `GET /comments/post/:postId`: comentarios visibles recientes para un post
- `POST /comments`: crear comentario

### Etiquetas
- `GET /tags`: lista todas las etiquetas

---

## ℹ️ Notas

- El proyecto utiliza una base de datos SQLite local (`database.sqlite`), ya preconfigurada.
- Se incluye el paquete `cors` habilitado, para permitir llamadas desde React.
