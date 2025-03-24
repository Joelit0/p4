# Recipes API

API REST desarrollada con **Spring Boot** para gestionar recetas. Permite crear, leer, actualizar y eliminar recetas.

##  Endpoints

| Método  | Ruta                | Cuerpo (JSON) | Descripción | Respuestas posibles |
|---------|---------------------|---------------|-------------|---------------------|
| **GET** | `/api/recipes` | No | Obtiene todas las recetas | `200 OK` Devuelve la lista de recetas |
| **GET** | `/api/recipes/{id}` | No | Obtiene una receta por ID | `200 OK` La receta coincidente/ `404 Not Found` Si no existe la receta |
| **POST** | `/api/recipes` | Si | Crea una nueva receta | `201 Created` Receta creada / `400 Bad Request` Alygun dato inválido en la request |
| **PUT** | `/api/recipes/{id}` | Si | Actualiza una receta por ID | `200 OK` La receta actualizada / `404 Not Found` Si no existe la receta |
| **DELETE** | `/api/recipes/{id}` | No | Elimina una receta por ID | `204 No Content` Borrado exitoso / `404 Not Found` Si no existe la receta |

## Ejemplo de Cuerpo JSON (POST/PUT)

```json
{
  "name": "Tortilla de Papas",
  "ingredients": ["Papas", "Huevos", "Sal", "Aceite"],
  "description": "Receta clásica de tortilla española.",
  "imageUrl": "https://misrecetas.com/tortilla.jpg",
  "videoUrl": "https://www.youtube.com/watch?v=abcd1234"
}
```

# Pruebas en Postman

## GET
## SHOW
  Es decir un get de un recurso específico
  
## POST

## UPDATE

## DELETE
