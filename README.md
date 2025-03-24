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
![GET](https://github.com/user-attachments/assets/5114de06-d6c5-4ce9-8ba1-e7906beb3389)

## SHOW
  Es decir un get de un recurso específico
  
  ![SHOW](https://github.com/user-attachments/assets/13e3d2b5-e4f0-487d-99ba-4cb6cca126a6)

## POST
![POST](https://github.com/user-attachments/assets/2a535110-6445-4ac4-b059-ed44ab7c6499)

## UPDATE
![UPDATE](https://github.com/user-attachments/assets/74348fca-2289-4c66-96b7-70881d2e15cd)

## DELETE
![DELETE](https://github.com/user-attachments/assets/550a6475-df84-4310-a218-49e0776b3385)

