![forogun](https://github.com/Danmargiela/foro_hub_final/assets/16968289/b46d68a9-ae8d-4b74-8b2d-16cb617cf1e5)

# ForoHub

Bienvenido a ForoHub, una API REST para un foro construida con Spring Boot. Este proyecto es parte del desafío final de **Practicando Spring Framework: Challenge Foro Hub**. Permite a los usuarios registrarse, iniciar sesión, crear tópicos y responder a ellos, todo gestionado de manera segura con autenticación JWT.

## Índice

- [Características](#características)
- [Tecnologías Utilizadas](#tecnologías-utilizadas)
- [Requisitos Previos](#requisitos-previos)
- [Configuración](#configuración)
- [Endpoints](#endpoints)
- [Contribución](#contribución)
- [Autor](#autor)
- [Licencia](#licencia)

## Características

- Registro y autenticación de usuarios.
- Creación y gestión de tópicos.
- Autenticación segura con JWT.
- Endpoints protegidos.
- Documentación API con Swagger.

## Tecnologías Utilizadas

- Java 17
- Spring Boot
- Spring Security
- JWT (JSON Web Tokens)
- JPA (Java Persistence API)
- Hibernate
- MySQL
- Lombok
- Flyway
- Swagger

## Requisitos Previos

- Java 17
- Maven
- MySQL

## Configuración

Configura la base de datos MySQL y actualiza el archivo `application.properties` con tus credenciales:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/forohub
spring.datasource.username=root
spring.datasource.password=root1234
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true

spring.h2.console.enabled=true

jwt.secret=mysecretkey
jwt.expiration=86400000
```

## Endpoints

- `POST /users`: Registrar un nuevo usuario.
- `POST /login`: Iniciar sesión y obtener un token JWT.
- `POST /topics`: Crear un nuevo tópico.
- `GET /topics`: Listar todos los tópicos.
- `DELETE /topics/{id}`: Eliminar un tópico por ID.

## Contribución

¡Contribuciones son bienvenidas! Por favor, abre un issue o envía un pull request.

## Autor

**Daniel Sánchez**

- [GitHub](https://github.com/Danmargiela)

## Licencia

Este proyecto está licenciado bajo la Licencia MIT - ver el archivo [LICENSE](LICENSE) para más detalles.
