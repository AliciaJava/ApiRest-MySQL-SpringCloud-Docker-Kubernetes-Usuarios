
# Microservicio de Usuarios – Spring Cloud & Kubernetes

Microservicio `msvc-usuarios` construido con **Spring Boot 3**, **Spring Cloud**, **PostgreSQL/MySQL**, **Docker** y **Kubernetes**.  
Forma parte de un ecosistema de microservicios que usa **OpenFeign** para comunicación inter-servicios.

---

## Stack Tecnológico

| Tecnología        | Versión |
|-------------------|---------|
| Java              | 21      |
| Spring Boot       | 3.5.6   |
| Spring Cloud      | 2025.0.0|
| Spring Data JPA   | Latest  |
| OpenFeign         | Latest  |
| PostgreSQL / MySQL| 15+ / 8+|
| JUnit             | 5       |

---

## Instalación Rápida

```bash
git clone https://github.com/tu-usuario/msvc-usuarios.git
cd msvc-usuarios
```

Configura `application.properties` con tu BD y ejecuta:

```bash
mvn clean install
mvn spring-boot:run
```

Servicio levantado en: [http://localhost:8001](http://localhost:8001)

---

## Endpoints REST

| Método | Endpoint           | Descripción               |
|--------|--------------------|---------------------------|
| GET    | `/usuarios`        | Listar todos              |
| GET    | `/usuarios/{id}`   | Obtener por ID            |
| POST   | `/usuarios`        | Crear usuario             |
| PUT    | `/usuarios/{id}`   | Actualizar usuario        |
| DELETE | `/usuarios/{id}`   | Eliminar usuario          |

---

## Testing

```bash
mvn test
```

---

## 📸 Evidencias

| Contexto | Imagen |
|----------|--------|
| Servicio levantado | ![RUN US](https://github.com/user-attachments/assets/548ee97c-32c0-4d3f-b238-988ee6ee7c5c) |
| Swagger / Health | ![LOCALHOST](https://github.com/user-attachments/assets/6d6185e8-71e8-4726-bb85-f5748e160316) |
| Base de datos | ![MySQL Workbench](https://github.com/user-attachments/assets/5974c847-47f2-4e35-a5ca-c72b60131db6) |
| Pruebas Postman | ![Postman](https://github.com/user-attachments/assets/13ddbc75-693c-4425-a805-19f9a48f93bb) |

---

## Roadmap del Proyecto

| Fase | Objetivo | Estado |
|------|----------|--------|
| ✅ Fase 1 | Microservicio Usuarios con MySQL/PostgreSQL | **Completado** |
| 🚧 Fase 2 | Microservicio Cursos con PostgreSQL | **En desarrollo** |
| 📋 Fase 3 | Validaciones y manejo global de errores | **Pendiente** |
| 📋 Fase 4 | Comunicación entre microservicios con OpenFeign | **Pendiente** |
| 📋 Fase 5 | Dockerización de cada microservicio | **Pendiente** |
| 📋 Fase 6 | Orquestación con Kubernetes | **Pendiente** |

---

## Contacto

**Alicia Ortega**  
📧 [Aliciaortega1986@gmail.com](mailto:Aliciaortega1986@gmail.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/aliciaortegamuñoz)

---

Este proyecto forma parte de mi portafolio profesional como **Java Developer especializada en microservicios con Spring Cloud**.  
Está activamente en desarrollo y se irá actualizando conforme avanzo en el roadmap.

---



