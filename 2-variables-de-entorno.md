# Variables de Entorno
### ¿Qué son las variables de entorno
Las variables de entorno son parámetros que contienen información sobre el entorno en el que se está ejecutando un programa o proceso. <br> 
Estas variables son útiles para almacenar datos que se utilizan en diferentes procesos o aplicaciones, como configuraciones, credenciales, o rutas a archivos importantes.<br>
En Docker, las variables de entorno se pueden pasar a los contenedores durante su creación para configurar el comportamiento de la aplicación en ejecución. Estas variables son accesibles dentro del contenedor.

### Para crear un contenedor con variables de entorno?

```
docker run -d --name <nombre contenedor> -e <nombre variable1>=<valor1> -e <nombre variable2>=<valor2>
```

### Crear un contenedor a partir de la imagen de nginx:alpine con las siguientes variables de entorno: username y role. Para la variable de entorno rol asignar el valor admin.

![Imagen](img/7.png)

# CAPTURA CON LA COMPROBACIÓN DE LA CREACIÓN DE LAS VARIABLES DE ENTORNO DEL CONTENEDOR ANTERIOR
![Imagen](img/8.png)
### Crear un contenedor con mysql:8 , mapear todos los puertos
![Imagen](img/9.png)

### ¿El contenedor se está ejecutando?
![Imagen](img/10.png)

### Identificar el problema
El contenedor se está ejecuntado de manera correcta y no existe problema.

### Eliminar el contenedor creado con mysql:8 
![Imagen](img/11.png)

### Para crear un contenedor con variables de entorno especificadas
- Portabilidad: Las aplicaciones se vuelven más portátiles y pueden ser desplegadas en diferentes entornos (desarrollo, pruebas, producción) simplemente cambiando el archivo de variables de entorno.
- Centralización: Todas las configuraciones importantes se centralizan en un solo lugar, lo que facilita la gestión y auditoría de las configuraciones.
- Consistencia: Asegura que todos los miembros del equipo de desarrollo o los entornos de despliegue utilicen las mismas configuraciones.
- Evitar Exposición en el Código: Mantener variables sensibles como contraseñas, claves API, y tokens fuera del código fuente reduce el riesgo de exposición accidental a través del control de versiones.
- Control de Acceso: Los archivos de variables de entorno pueden ser gestionados con permisos específicos, limitando quién puede ver o modificar la configuración sensible.

Previo a esto es necesario crear el archivo y colocar las variables en un archivo, **.env** se ha convertido en una convención estándar, pero también es posible usar cualquier extensión como **.txt**.
```
docker run -d --name <nombre contenedor> --env-file=<nombreArchivo>.<extensión> <nombre imagen>
```
**Considerar**
Es necesario especificar la ruta absoluta del archivo si este se encuentra en una ubicación diferente a la que estás ejecutando el comando docker run.

### Crear un contenedor con mysql:8 , mapear todos los puertos y configurar las variables de entorno mediante un archivo
![Imagen](img/12.png)

# CAPTURA CON LA COMPROBACIÓN DE LA CREACIÓN DE LAS VARIABLES DE ENTORNO DEL CONTENEDOR ANTERIOR 
![Imagen](img/13.png)
### ¿Qué bases de datos existen en el contenedor creado?
![Imagen](img/14.png)
