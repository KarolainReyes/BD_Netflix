# 📚 Base de Datos de Seguimiento de Contenido Multimedia

Este proyecto consiste en el **diseño de una base de datos NoSQL** utilizando **MongoDB**, destinada a registrar el progreso de usuarios al ver series, películas o leer libros.

> El sistema no incluye funcionalidades CRUD ni lógica de aplicación. Únicamente contiene los archivos `.json` necesarios para poblar la base de datos.

---

## 🧠 Descripción General

La base de datos permite representar información relacionada con:

- Usuarios registrados.
- Recursos multimedia (libros, películas, series).
- Valoraciones, reseñas y estados de progreso.
- Géneros, formatos, editoriales y plataformas asociadas.

---

## 🗂️ Estructura de Colecciones y Archivos JSON

| Colección         | Archivo JSON                              | Descripción breve                                        |
|------------------|-------------------------------------------|----------------------------------------------------------|
| `usuarios`        | `Contenido_multimedia.usuarios.json`      | Información básica de los usuarios.                      |
| `editoriales`     | `Contenido_multimedia.editoriales.json`   | Editoriales asociadas a libros.                          |
| `formatos`        | `Contenido_multimedia.formatos.json`      | Tipo de recurso: libro, película o serie.                |
| `generos`         | `Contenido_multimedia.generos.json`       | Géneros como acción, comedia, drama, etc.                |
| `plataformas`     | `Contenido_multimedia.plataformas.json`   | Plataformas donde se puede ver el recurso (Netflix, etc).|
| `recursos`        | `Contenido_multimedia.recursos.json`      | Recursos agregados por los usuarios con estado, reseñas y más. |

---

## 🛠️ Comandos para crear la base de datos en MongoDB

```bash
use contenido_multimedia

db.usuarios.insertMany(<Contenido_multimedia.usuarios.json>)
db.editoriales.insertMany(<Contenido_multimedia.editoriales.json>)
db.formatos.insertMany(<Contenido_multimedia.formatos.json>)
db.generos.insertMany(<Contenido_multimedia.generos.json>)
db.plataformas.insertMany(<Contenido_multimedia.plataformas.json>)
db.recursos.insertMany(<Contenido_multimedia.recursos.json>)
```



---

## 👩‍💻 Desarrollado por

 * [Karol Reyes](https://github.com/KarolainReyes)

 * [Andres Leal](https://github.com/Andre07g)

---

## 🧩 Requisitos

- MongoDB instalado localmente o acceso a MongoDB Atlas.
- MongoDB Compass (opcional, para inspeccionar visualmente las colecciones).

---

## 📝 Licencia

Este proyecto es de uso educativo. Puede ser utilizado como referencia para modelado de bases de datos NoSQL en MongoDB.