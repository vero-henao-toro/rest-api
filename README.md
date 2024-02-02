Para la realización del ejemplo usé la librería MUX que permite definir rutas y métodos HTTP para responder a ellos, de una manera fácil, para la conexión y comunicación con Postgres se utilizó el ORM GROM:

Para realizar la conexión a la base de datos se necesitan realizar los siguientes pasos:

Descargar Docker
En la linea de commandos ejecutar lo siguiente para crear la imagen de postgres:docker run --name some-postgres -e POSTGRES_USER=admin -e POSTGRES_PASSWORD=admin123 -p 5432:5432 -d postgres
Para conectarnos al contenedor ejecutar : docker ps
Ejecutar el siguiente comando para establecer el modo interactivo del contenedor: docker exec -it some-postgres bash
Ejecutar el siguiente comando para conectarnos a la BD: psql -U admin --password
Crear la BD con el siguiente comando: CREATE DATABASE gorm;
