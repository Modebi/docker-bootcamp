# Fichero Dockerfile inicial.
Primer día aprendiendo Docker en la bootcamp.

## Construir la imagen.
`
docker build . -t miapache
`
## Ejecutar la imagen.
Ejecutar la imagen con bindeo de puertos.
`
docker run -d --name contenedor1 -p 8080:80 miapache
`
# Ejecutar la imagen asignándole un volumen.
`
docker run -v volume:/usr/local/apache2 -d --name contenedor1 -p 8080:80 miapache
`

## Comandos útiles aprendidos
