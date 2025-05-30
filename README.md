# Inventario - El Tornillo Feliz 🛠️

Bienvenido al proyecto **"Inventario El Tornillo Feliz"**, un sistema web pensado para gestionar productos en una ferretería de forma simple, eficiente y moderna. Desarrollado con ❤️ por un jardinero curioso que programó con pasión.

---

## 🌐 Tecnologías utilizadas

### Backend:

* Java 17
* Spring Boot
* Maven
* Spring Data JPA
* H2 Database (modo dev)
* PostgreSQL (modo prod)

### Frontend:

* HTML5 + CSS3
* JavaScript
* Bootstrap 5
* Font Awesome

---

## ⚙️ Funcionalidades actuales

### Backend:

* CRUD completo de productos.
* Alerta de productos con bajo stock.
* API REST bajo `/api/productos`:

  * `GET /api/productos` – Listar todos.
  * `GET /api/productos/bajo-stock?limite=10` – Ver productos con bajo stock.
  * `POST /api/productos` – Agregar nuevo.
  * `PUT /api/productos/{id}` – Editar producto.
  * `DELETE /api/productos/{id}` – Eliminar producto.

### Frontend:

* Vista principal con tabla dinámica de productos.
* Botón para ver productos con bajo stock.
* Formulario para agregar nuevo producto.
* Formulario para editar producto.
* Notificación visual de bajo stock.

---

## 📦 Cómo correr el proyecto localmente

### Backend (Spring Boot)

```bash
./mvnw spring-boot:run
```

Corre en `http://localhost:8080`

### Frontend (Live Server VSCode)

Abre la carpeta `/frontend` con VS Code y usa la extensión Live Server para abrir `index.html`.

---

## 🧪 Test desde REST Client

Si usás VS Code, podés crear un archivo `test.http`:

```http
### Listar productos
GET http://localhost:8080/api/productos

### Ver bajo stock (límite 5)
GET http://localhost:8080/api/productos/bajo-stock

### Agregar producto
POST http://localhost:8080/api/productos
Content-Type: application/json

{
  "codigo": "ABC123",
  "nombre": "Martillo",
  "cantidad": 3,
  "precio": 45.00
}

### Eliminar producto
DELETE http://localhost:8080/api/productos/1
```

---

## 📸 Capturas de pantalla

* Tabla con productos.
* Formulario limpio para agregar.
* Todo con diseño responsivo.

> ¡Y sí! Muy pronto le sumamos login de usuarios y un dashboard que te haga sentir en casa. 🛠️🧑‍💻

---

## 🚀 Próximamente

* Módulo de usuarios (login y roles).
* Dashboard de métricas (productos más vendidos, estadísticas).
* Control de auditoría (quién editó qué).

---

## 🙌 Autor

**Gustavo** – Jardinero y Programador 🌿💻

> "De la tierra al código, todo se puede sembrar y hacer crecer."

GitHub: [https://github.com/mipa57](https://github.com/mipa57)

---

¡Con tu feedback hacemos crecer esta herramienta aún más! 🌱
