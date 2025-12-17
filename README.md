
# ApiRestSpringCloud-PostgreSQL-Docker-Kubernetes

Proyecto **Spring Boot** con **Spring Cloud**, PostgreSQL/MySQL, Docker y Kubernetes. Este microservicio (`msvc-usuarios`) forma parte de un ecosistema de microservicios, utilizando OpenFeign para comunicación entre servicios.

# Microservicio Usuarios - Spring Cloud

Proyecto **Spring Cloud** con PostgreSQL/MySQL y Spring Boot.  
Actualmente en desarrollo como parte del aprendizaje de microservicios con Spring Cloud.

---

## Tecnologías utilizadas

- Java 21
- Spring Boot 3.5.6
- Spring Cloud 2025.0.0
- Spring Data JPA
- Spring Cloud OpenFeign
- PostgreSQL / MySQL
- JUnit para testing

---

## Configuración e instalación

Sigue estos pasos para ejecutar el proyecto en tu máquina local:

### 1. Clonar el repositorio

```bash
git clone https://github.com/tu-usuario/msvc-usuarios.git
cd msvc-usuarios
````

### 2. Configurar la base de datos

* **MySQL**: Actualiza `application.properties` con tus credenciales.
* **PostgreSQL**: Ajusta la URL, usuario y contraseña si prefieres usar PostgreSQL.

Ejemplo (`application.properties`):

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/usuarios_db
spring.datasource.username=root
spring.datasource.password=root
spring.jpa.hibernate.ddl-auto=update
```

### 3. Ejecutar el proyecto

Desde la raíz del proyecto:

```bash
mvn clean install
mvn spring-boot:run
```

El microservicio estará disponible en:

```
http://localhost:8080
```

---

## Endpoints principales

* `GET /usuarios` - Listar todos los usuarios
* `GET /usuarios/{id}` - Obtener usuario por ID
* `POST /usuarios` - Crear un nuevo usuario
* `PUT /usuarios/{id}` - Actualizar un usuario existente
* `DELETE /usuarios/{id}` - Eliminar un usuario

---

## Testing

Ejecutar tests unitarios y de integración:

```bash
mvn test
```

---

## Próximos pasos de aprendizaje

* Integrar Docker para contenerización
* Implementar Kubernetes para despliegue
* Agregar más microservicios y comunicación con Spring Cloud

## Autor

**Nombre:** Alicia Ortega  
**Email:** [Aliciaortega1986@gmail.com](mailto:Aliciaortega1986@gmail.com)  

---

## Licencia

Este proyecto está bajo la licencia **MIT**.
Consulta el archivo [LICENSE](LICENSE) para más detalles.


