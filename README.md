
# ApiRestSpringCloud-PostgreSQL-Docker-Kubernetes

Proyecto **Spring Boot** con **Spring Cloud**, PostgreSQL/MySQL, Docker y Kubernetes. Este microservicio (`msvc-usuarios`) forma parte de un ecosistema de microservicios, utilizando OpenFeign para comunicación entre servicios.

---

## Tecnologías utilizadas

- Java 21
- Spring Boot 3.5.6
- Spring Cloud 2025.0.0
- Spring Data JPA
- Spring Web
- Spring Cloud OpenFeign
- MySQL
- Docker
- Kubernetes

---

## Requisitos

- Java 21
- Maven 4+
- Docker
- Minikube o un cluster Kubernetes
- MySQL/PostgreSQL

---

## Instalación y ejecución

1. Clona el repositorio:
   ```bash
   git clone <URL_DEL_REPOSITORIO>
   cd msvc-usuarios
````

2. Configura la base de datos en `application.properties`:

   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/usuarios
   spring.datasource.username=root
   spring.datasource.password=tu_contraseña
   spring.jpa.hibernate.ddl-auto=update
   ```

3. Ejecuta el proyecto localmente:

   ```bash
   mvn spring-boot:run
   ```

4. Para Docker:

   ```bash
   docker build -t msvc-usuarios .
   docker run -p 8080:8080 msvc-usuarios
   ```

5. Para Kubernetes (ejemplo con Minikube):

   ```bash
   kubectl apply -f k8s/deployment.yaml
   kubectl apply -f k8s/service.yaml
   ```

---

## Endpoints

Ejemplo de endpoints REST disponibles:

| Método | Endpoint       | Descripción               |
| ------ | -------------- | ------------------------- |
| GET    | /usuarios      | Listar todos los usuarios |
| GET    | /usuarios/{id} | Obtener usuario por ID    |
| POST   | /usuarios      | Crear un nuevo usuario    |
| PUT    | /usuarios/{id} | Actualizar usuario        |
| DELETE | /usuarios/{id} | Eliminar usuario          |

---

## Autor

**Alicia Ortega**
Email: [Aliciaortega1986@gmail.com](mailto:Aliciaortega1986@gmail.com)

---

## Licencia

Este proyecto está bajo la licencia **MIT**.
Consulta el archivo [LICENSE](LICENSE) para más detalles.


