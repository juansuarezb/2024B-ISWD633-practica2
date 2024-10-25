Antes de realizar la práctica, mis conocimientos sobre el manejo de contenedores con Docker y la configuración de bases de datos eran básicos. Sabía cómo crear contenedores, pero no tenía experiencia práctica con la interacción entre contenedores y herramientas específicas como Postgres y pgAdmin. Además, desconocía detalles clave sobre cómo gestionar variables de entorno en Docker, el uso de clientes para administrar bases de datos en un entorno contenedorizado, y la manipulación de datos en bases de datos SQL desde un cliente gráfico como pgAdmin.
He aprendido a:
Crear redes Docker de tipo bridge: Utilicé el comando docker network create para definir redes que permiten la interacción entre contenedores. 
Conectar contenedores a redes: Ahora sé cómo conectar y desconectar contenedores a redes específicas usando docker network connect y docker network disconnect.

Mapear puertos correctamente: Aprendí a utilizar la opción -p para mapear puertos del contenedor hacia la máquina host, permitiendo el acceso a servicios dentro del contenedor desde el navegador.

Persistencia de datos en bases de datos contenedorizadas: Al eliminar y recrear contenedores de aplicaciones como WordPress, pude observar que los datos persistían, siempre que la configuración de la base de datos y el almacenamiento de datos se gestionaran correctamente entre los contenedores.
