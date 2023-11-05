# Rust-Crud-Api

## Contenidos

1. [Introducción](#introducción)
2. [Requisitos Previos](#requisitos-previos)
3. [Configuración](#configuración)
4. [Instrucciones de Uso](#instrucciones-de-uso)

---

## Introducción

`Rust-Crud-Api` es una aplicación Rust que implementa una API CRUD (Crear, Leer, Actualizar, Eliminar) para interactuar con una base de datos PostgreSQL. Esta aplicación proporciona un servidor web que permite realizar operaciones básicas en una base de datos de usuarios, como crear, leer, actualizar y eliminar registros.

---


## Requisitos Previos

Antes de ejecutar esta aplicación, asegúrate de tener instalados los siguientes componentes:

- [Rust](https://www.rust-lang.org/tools/install): El lenguaje Rust y su administrador de paquetes Cargo.
- [Docker](https://www.docker.com/get-started): Para ejecutar la base de datos PostgreSQL en un contenedor.
- [Docker Compose](https://docs.docker.com/compose/install/): Para administrar los contenedores y servicios.

---

## Configuración

### Variables de Entorno

La aplicación utiliza una variable de entorno llamada `DATABASE_URL` para establecer la URL de conexión a la base de datos PostgreSQL. Asegúrate de configurar esta variable antes de ejecutar la aplicación. Puedes hacerlo en el archivo `docker-compose.yml` o proporcionarla directamente al construir la imagen Docker.

Ejemplo de URL de conexión:

```shell
DATABASE_URL=postgres://usuario:contraseña@host:puerto/nombre_basedatos
```
---

## Instrucciones de Uso

Siga estos pasos para ejecutar la aplicación:

1. Clona este repositorio en tu máquina local:

   ```shell
   git clone https://github.com/Dio-Bardo/Rust-Crud-Api.git
   ```
2. Crea un archivo .env en el directorio raíz del proyecto y define la variable de entorno DATABASE_URL con la URL de conexión a tu base de datos PostgreSQL:
   ```shell
   cd rust-crud-api
   ```
3. Ejecuta la aplicación utilizando Docker Compose:
   ```shell
   docker-compose up
4. Esto iniciará la aplicación y la base de datos PostgreSQL en contenedores separados.

La aplicación estará disponible en http://localhost:8080.
