# Docker Compose

## Que es ?

**Docker Compose** es una herramienta para definir y ejecutar aplicaciones de Docker de varios contenedores. En Compose, se usa un archivo YAML para configurar los servicios de la aplicación. 
Después, con un solo comando, se crean y se inician todos los servicios de la configuración.

## Archivo de Docker Compose
El archivo YAML define todos los servicios que se van a implementar.
Por defecto, el archivo Docker Compose tiene el siguiente nombre: **docker-compose.yaml**


### Iniciar/reiniciar todos los servicios definidos en el archiov docker-compose.yaml

    docker-compose up

La primera vez que se ejecuta el comando, se extraen las imagenes configuradas en el node **services**, y luego las descarga y las monta.


### Comprobación de la disponibilidad del servicio

Se puede usar el comando **docker images** para enumerar las imagenes de contenedor descargadas.


### Ejecutar comandos en un contenedor

Con la siguiente instruccion, podemos ejecutar un comando dentro de un contenedor/servicio.

    docker compose exec <nombre contenedor> sh


## Comandos utiles

Listar contenedores en ejecucion. Para listar los contenedores en ejecución y parados usamos el parametro -a

```
docker ps -a
```

Listar imagenes descargadas en local

```
docker images
```
