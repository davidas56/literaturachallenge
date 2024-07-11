# Biblioteca API

## Descripción

Esta API permite realizar operaciones básicas sobre una colección de libros. Las operaciones incluyen la consulta, adición y eliminación de libros. Está construida utilizando [insertar lenguaje/framework aquí].

## Endpoints

### Obtener lista de libros

- **URL:** `/books`
- **Método:** `GET`
- **Descripción:** Obtiene la lista de todos los libros disponibles.
- **Respuesta exitosa:**
  - **Código:** 200 OK
  - **Contenido:**
    ```json
    [
      {
        "id": 1,
        "title": "Título del libro",
        "author": "Autor del libro"
      },
      ...
    ]
    ```

### Obtener un libro por ID

- **URL:** `/books/{id}`
- **Método:** `GET`
- **Descripción:** Obtiene la información de un libro específico por ID.
- **Parámetros de ruta:**
  - `id` (requerido): ID del libro.
- **Respuesta exitosa:**
  - **Código:** 200 OK
  - **Contenido:**
    ```json
    {
      "id": 1,
      "title": "Título del libro",
      "author": "Autor del libro"
    }
    ```
- **Respuesta de error:**
  - **Código:** 404 Not Found
  - **Contenido:**
    ```json
    {
      "error": "Libro no encontrado"
    }
    ```

### Agregar un nuevo libro

- **URL:** `/books`
- **Método:** `POST`
- **Descripción:** Agrega un nuevo libro a la colección.
- **Cuerpo de la solicitud:**
  - **Contenido:**
    ```json
    {
      "title": "Título del libro",
      "author": "Autor del libro"
    }
    ```
- **Respuesta exitosa:**
  - **Código:** 201 Created
  - **Contenido:**
    ```json
    {
      "id": 1,
      "title": "Título del libro",
      "author": "Autor del libro"
    }
    ```




## Uso

Una vez que el servidor esté en funcionamiento, puedes interactuar con la API utilizando herramientas como [Postman](https://www.postman.com/) o `curl`.



[Insertar información de la licencia aquí]
