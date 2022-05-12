# Fichero Dockerfile inicial.
Primer día aprendiendo Docker en la bootcamp.

## Construir la imagen.
`
docker build . -t miapache
`
## Ejecutar la imagen.
Ejecutar la imagen con bindeo de puertos y en segundo plano.
`
docker run -d --name contenedor1 -p 8080:80 miapache
`
## Ejecutar la imagen asignándole un volumen.
Además de lo anterior, le asignamos un volumen.
`
docker run -v volume:/usr/local/apache2 -d --name contenedor1 -p 8080:80 miapache
`
## Acceder a la imagen con bash.
`
docker exec -it ID_CONTENEDOR bash
`

## Comandos útiles aprendidos
Construir una imagen desde un Dockerfile: `docker build`


Procesos ejecutados por Docker: `docker ps`


Descargar una imagen: `docker pull`


Listar imagenes: `docker image ls`


Listar contenedores: `docker container ls`


Eliminar imágenes: `docker rmi`


Eliminar contenedores: `docker rm`


