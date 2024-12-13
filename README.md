# Sistema de Gestión de Pacientes Veterinarios
## Descripción
Este proyecto consiste en desarrollar un sistema de gestión de pacientes para la clínica veterinaria de Margarita. El sistema permitirá a Margarita y su equipo listar, agregar, editar y eliminar pacientes, gestionar citas y mantener un registro organizado de los tratamientos realizados.
La aplicación se implementará en Java utilizando el framework Spring Boot y almacenará los datos en una base de datos en memoria (H2 Database) o en MySQL dockerizada. Además, se incluirá una API REST para facilitar la integración con el frontend.
---
## Objetivos del Proyecto
1. Reforzar los conceptos de programación orientada a objetos (POO).
2. Aplicar principios de encapsulamiento para proteger los datos.
3. Diseñar un diagrama de flujo que explique el funcionamiento del sistema.
4. Desarrollar el sistema conforme al diagrama planteado.
---
## Requisitos Funcionales
### Gestión de Pacientes:
- Listar, agregar, editar y eliminar pacientes.
- Cada paciente debe tener un perfil con la siguiente información:
  - Nombre
  - Edad
  - Raza
  - Género
  - Número de identificación
  - Nombre y apellidos del tutor
  - Número de teléfono del tutor
- Acceso a los datos de un paciente mediante su número de identificación.
- Registro de tratamientos realizados para cada paciente.
### Gestión de Citas:
- Listar, agregar, editar y eliminar citas.
- Cada cita debe incluir:
  - Fecha y hora
  - Paciente asociado
  - Tipo de consulta (estándar/urgencia)
  - Motivo de la cita
  - Estado de la cita (pendiente/pasada)
---
## Requisitos Técnicos
1. Conocimientos en Java y Spring Boot.
2. Aplicación de buenas prácticas de desarrollo.
3. Implementación de tests unitarios para modelos, servicios y controladores.
4. Cobertura de testing mínima del 70%.
5. Normalización de tablas en la base de datos.
6. Arquitectura backend bien definida con separación de capas.
---
## Tecnologías Utilizadas
- Lenguaje: **Java**
- Framework: **Spring Boot**
- Base de datos: **H2 Database** / **MySQL dockerizada**
- Almacenamiento de archivos: **Firebase Storage**
- Contenedores: **Docker**
- Testing: **JUnit**, **Mockito**
---
## Instrucciones de Instalación y Uso
### Requisitos Previos:
- Tener instalado **Java 17** o superior.
- Docker (para MySQL dockerizada).
### Pasos:
1. Clonar el repositorio desde GitHub:
   ```bash
   git clone https://github.com/<tu-usuario>/sistema-veterinario.git
   cd sistema-veterinario
   ```
2. Configurar la base de datos en el archivo `application.properties`:
   - Para H2 Database:
     ```properties
     spring.datasource.url=jdbc:h2:mem:testdb
     spring.datasource.driver-class-name=org.h2.Driver
     spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
     ```
   - Para MySQL dockerizada:
     ```properties
     spring.datasource.url=jdbc:mysql://localhost:3306/veterinaria
     spring.datasource.username=root
     spring.datasource.password=root
     ```
3. Construir y ejecutar el proyecto:
   ```bash
   ./mvnw spring-boot:run
   ```
4. Acceder a la aplicación en `http://localhost:8080`.
---
## Colaboradores
- Fuad Hussein
- Jose Manuel
- Yuliana Alcalá
- Clara Vilera
- Angelo Colmenares 
