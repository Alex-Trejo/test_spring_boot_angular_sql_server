# Alex Fernando Trejo Duque

## **Implementación**

### **Backend**

El backend del proyecto fue implementado utilizando **Spring Boot 3.2.6**, junto con las siguientes tecnologías y herramientas:

- **Spring Security**: Gestión de seguridad y autenticación mediante **JWT (JSON Web Tokens)**.
- **Liquibase**: Gestión de migraciones de base de datos, asegurando que las estructuras de las tablas estén siempre actualizadas.
- **JPA (Java Persistence API) con Hibernate**: Manipulación de la base de datos utilizando un enfoque ORM (Object-Relational Mapping).
- **Refresh Token**: Implementación de un flujo de autenticación más seguro, permitiendo renovar el token de acceso sin necesidad de volver a iniciar sesión.
- **JpaRepository**: Interfaz de repositorio de Spring Data JPA, simplificando las operaciones de acceso a datos y la interacción con la base de datos.
- **Arquitectura Limpia (Clean Architecture)**: 
  La aplicación sigue una estructura modular basada en capas, donde se separan las responsabilidades en distintas áreas del sistema. Este enfoque facilita el mantenimiento, la escalabilidad y las pruebas del sistema. Se organizaron las clases en las siguientes capas principales:
  - **Capa de presentación**: Controladores (Resolvers GraphQL) que gestionan las solicitudes de los usuarios.
  - **Capa de lógica de negocio**: Servicios que implementan la lógica del negocio.
  - **Capa de acceso a datos**: Repositorios que interactúan con la base de datos utilizando Spring Data JPA.
  - **Capa de configuración**: Configuraciones de seguridad (JWT, Spring Security, CORS) y configuración de GraphQL.

Para más detalles sobre cómo ejecutar el proyecto, configuraciones y dependencias, consulta la carpeta `backend`.
