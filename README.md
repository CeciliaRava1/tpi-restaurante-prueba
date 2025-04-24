# tpi-restaurante-prueba
1 : Descargamos la imagen de postgres
docker pull postgres

2 : Creamos un contenedor con la imagen de postgres
docker run --name postgres-db -e POSTGRES_PASSWORD=mipassword -d postgres

3: Verificamos si está corriendo
docker ps

4: Accedemos al bash de nuestro contenedor
docker exec -it postgres-db psql -U postgres

5 : Creamos la base de datos
CREATE DATABASE mi_base_de_datos