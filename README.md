# DOCKER

- Crear y ejecutar contenedores.

### Comandos:
```shell
# Ver contenedores en ejecucion
$ docker ps
```


## Contenedor

- "Pieza de software" que permite ejecutar de manera aislada uno o varios procesos.
- Utiliza el kernel del sistema operativo.
- Se crea a partir de una imagen base (Docker Image).

### Comandos:
```shell
# Crear un nuevo contenedor a apartir de una imagen
$ docker run <image name>

# Deteneder ejecucion de un contenedor
$ docker stop <container>

# Eliminar un contenedor
$ docker rm <container> 
```


## Dokcer image

- Plantilla que contiene lo necesario para ejecutar un contenedor.
- Se construyen usando un Dockerfile.
- Son inmutables.
- Se pueden crear con base en otras imagenes.
- Pueden tener diferentes versiones (tags).

### Comandos:
```shell
# Ver lista de imagenes disponibles locales
$ docker images

# Eliminar una imagen
$ docker rmi <image>

# Descargar una imagen de docker hub
$ docker pull <image>
```


## Dockerfile

- Archivo de texto con las instrucciones de instalacion de las dependencias.
- Permite definir como se va a ejecutar el proceso principal dentro del contenedor.
- Requiere un proceso de compilacion para construir la imagen final.

### Comandos:
```shell
# Construir una nueva imagen a partir de un Dockerfile
$ docker build -t <image_tag>
```
