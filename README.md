# Backend encuentas NDT

Necesitamos crear un backend con las siguientes características:
- Servir archivos estáticos (index. login visualizaciones...)
- Poder almacenar valoraciones

## Base de datos

Utilizamos SQLite con dos tablas:
    -users:
        - name
        - password
    -reviews
        - rating
        - opinions/message

## api

### POST /api/reviews?

Endpoint para recibir los datos del usuario, los mandaremos por el body en formato JSON

```json
{
    "rating": "good",
    "message": "lo que sea"
}
```
En rating solo pueden llegar tres valores posibles:

- good
- neutral
- bad

En message:

- Máximo 256 caracteres

