# Título del Proyecto

**ForoHub**

## Descripción del Proyecto

*ForoHub es una aplicación de foro diseñada para gestionar temas, usuarios y discusiones de manera eficiente. Proporciona endpoints para crear, actualizar, eliminar y visualizar temas. La aplicación está construida utilizando Spring Boot e integra una base de datos PostgreSQL. La seguridad se gestiona utilizando autenticación JWT.*

## Características
    -Registro y autenticación de usuarios.
    -Operaciones CRUD para temas.
    -Paginación y ordenación de listas de temas.
    -Validación para integridad y consistencia de datos.
    -Gestión detallada de errores y respuestas.

## Instalación y Requisitos Previos
    -Java 11 o superior
    -Maven
    -PostgreSQL

## Pasos de Instalación
Clona el repositorio:

[git clone] (https://github.com/AdrianHdz21/ Challenge_ForoHub)

```bash 
cd challenge.ForoHub
```

## Configura la base de datos:

Crea una base de datos PostgreSQL y configura las credenciales en el archivo application.properties.

properties

spring.datasource.url=jdbc:postgresql://<HOST_BD>/<NAME_DB>
spring.datasource.username=<USUARIO>
spring.datasource.password=<CONTRASEÑA>

## Instala las dependencias:

```bash
mvn clean install
```

## Ejecuta la aplicación:

```bash
mvn spring-boot:run
```

## Uso
Endpoints Principales

*Autenticación de Usuario:*

    http://localhost:8080/login
    Metodo:POST 

*Crear un Topico:*

    http://localhost:8080/topicos
    Metodo:POST 

*Actualizar un Topico:*

    http://localhost:8080/topicos
    Metodo:PUT

*Eliminar un Tema:*

    http://localhost:8080/topicos/{id}
    Metodo: DELETE 

*Listar Topicos:*

    http://localhost:8080/topicos
    Metodo: GET

## Ordenación y Paginación

Los temas seran listados con paginación y ordenados por fecha de creación y curso en orden descendente (del más nuevo al más viejo):

## Contribución
-Haz un fork del repositorio

-Crea una nueva rama:

```bash
git checkout -b mi-rama
```

-Realiza tus cambios y haz commits:

```bash
git commit -m "Descripción de mis cambios"
```

-Sube tus cambios a tu fork:

```bash
git push origin mi-rama
```

-Abre un Pull Request en el repositorio original
