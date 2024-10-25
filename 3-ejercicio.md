### Crear contenedor de Postgres sin que exponga los puertos. Usar la imagen: postgres:11.21-alpine3.17
![Imagen](img/15.png)
### Crear un cliente de postgres. Usar la imagen: dpage/pgadmin4

![Imagen](img/16.png)
La figura presenta el esquema creado en donde los puertos son:
- a: 5050
- b: 80
- c: 5432

![Imagen](img/esquema-ejercicio3.PNG)

## Desde el cliente
### Acceder desde el cliente al servidor postgres creado.
![Imagen](img/17.png)
![Imagen](img/18.png)
### Crear la base de datos info, y dentro de esa base la tabla personas, con id (serial) y nombre (varchar), agregar un par de registros en la tabla, obligatorio incluir su nombre.
![Imagen](img/19.png)
## Desde el servidor postgresl
### Acceder al servidor
### Conectarse a la base de datos info
![Imagen](img/20.png)
### Realizar un select *from personas
# AGREGAR UNA CAPTURA DE PANTALLA DEL RESULTADO
![Imagen](img/21.png)
