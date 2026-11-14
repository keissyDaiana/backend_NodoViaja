# 🌄 Nodo Viaja — Backend

Backend de **Nodo Viaja**, una plataforma web para dar a conocer sitios turísticos, gastronomía y hospedaje de **Garzón, Huila**.

![Node.js](logo.png)

---



## 🛠 Tecnologías

| Herramienta | Para qué se usa |
|---|---|
| **Node.js** | Ejecutar el servidor |
| **Express** | 
| **PostgreSQL** | Base de datos |
| **pg** | Conectar Node.js con PostgreSQL |
| **dotenv** | Leer las variables del archivo `.env` |
| **cors** | 
| **morgan** | Mostrar en consola cada petición que llega |

---


## 🔐 Variables de entorno

Crea un archivo `.env` en la raíz (puedes copiar `.env.example`) y completa tus datos:

```env
PORT=3000
NODE_ENV=development
PG_HOST=localhost
PG_PORT=5432
PG_DATABASE=proyecto
PG_USER=postgres
PG_PASSWORD=tu_clave_de_postgres
PG_MAX_POOL=10
PG_IDLE_TIMEOUT=30000
```

---

## 🗄 Base de datos

1.  Se Creo una base de datos llamada **`Database_NodoViaja`** en PostgreSQL.
2. Ejecuta el archivo `nodoviaja_postgres.sql` en esa base (con pgAdmin: *Query Tool* → pegar el contenido → ejecutar).

Esto crea las **27 tablas** de Nodo Viaja, organizadas en cuatro partes:

| Parte | Tablas principales |
|---|---|
| 👥 Usuarios y roles | `roles`, `usuarios`, `notificaciones` |
| 🧳 Turista | `reservas`, `favoritos`, `comentarios`, `ubicacion` |
| 🧳 Gastronomia | `reservas`, `menu`, `comentarios` |
| 🧳 Hospedaje | `reservas`, `comentarios` |
| 🏨 Administrador | `negocios`, `servicios`, `pagos`, `facturas`, `zonas`, `horarios_negocio`, `imagenes_negocio` |
| 🛡 Moderador | `solicitudes_aprobacion`, `verificaciones_contacto`, `avisos_mantenimiento`, `reportes_moderador`, `estadisticas_diarias` |

---

## 👩‍💻 Autores

- **Juan Stiven Jimenez - Keissy Benítez - Laura Parra - Johan Collada** — Aprendiz SENA, ADSO (ficha 3293992)

---

<p align="center">Hecho con ❤️ en Garzón, Huila</p>
