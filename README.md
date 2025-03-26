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


### **Frontend**

El frontend del proyecto fue implementado utilizando **Angular 19**, junto con las siguientes tecnologías y herramientas:

- **Angular**: Framework principal para la creación de la aplicación frontend, que sigue el patrón de arquitectura Modelo-Vista-Controlador (MVC).
- **GraphQL**: Implementación de consultas y mutaciones con GraphQL para interactuar con el backend, proporcionando una forma eficiente y flexible de obtener datos.
- **Apollo Client**: Cliente GraphQL utilizado para conectar con el servidor backend y gestionar las consultas y mutaciones de GraphQL en el frontend.
- **RxJS**: Biblioteca para programación reactiva, utilizada para manejar flujos de datos asincrónicos y eventos en Angular.
- **Angular Material**: Biblioteca de componentes UI para crear una interfaz de usuario moderna, responsiva y accesible.
- **SCSS (Sass)**: Preprocesador CSS utilizado para el estilo de la aplicación, permitiendo una estructura modular y reutilizable del código de estilos.
- **Guards y Interceptors**: Implementación de guards para protección de rutas y interceptores para manejar el token de autenticación (JWT) de forma segura.
- **Formularios Reactivos (Reactive Forms)**: Manejo de formularios en Angular de forma reactiva para garantizar un control eficiente y validaciones en tiempo real.
- **LocalStorage**: Se usa para almacenar el token JWT en el navegador del cliente una vez que el usuario ha iniciado sesión, lo que permite autenticar las solicitudes subsecuentes al backend.
- **Arquitectura Modular**: El proyecto sigue una arquitectura modular que agrupa funcionalidades en diferentes módulos para mejorar la organización, la reutilización y el mantenimiento del código.

Para más detalles sobre cómo ejecutar el proyecto, configuraciones y dependencias, consulta la carpeta `frontend`.