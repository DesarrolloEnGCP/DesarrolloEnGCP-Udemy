# Primeros Pasos con Cloud Shell y Docker.

## Comprobar version de Docker

```bash
docker --version
```

## Bajar y Ejecutar Imagen de Docker "Hola Mundo"
```bash
docker run hello-world
```
Unable to find image 'hello-world:latest' locally
latest: Pulling from library/hello-world
1b930d010525: Pull complete
Digest: sha256:6540fc08ee6e6b7b63468dc3317e3303aae178cb8a45ed3123180328bcc1d20f
Status: Downloaded newer image for hello-world:latest

Hello from Docker!
This message shows that your installation appears to be working correctly.

To generate this message, Docker took the following steps:
 1. The Docker client contacted the Docker daemon.
 2. The Docker daemon pulled the "hello-world" image from the Docker Hub.
    (amd64)
 3. The Docker daemon created a new container from that image which runs the
    executable that produces the output you are currently reading.
 4. The Docker daemon streamed that output to the Docker client, which sent it
    to your terminal.

To try something more ambitious, you can run an Ubuntu container with:
 $ docker run -it ubuntu bash

## Ver Imagenes Descargadas (la del paso anterior)
```bash
docker image ls
```

## Ver Contenedores (el modificar "--all" incluye los contenedores finalizados)
```bash
docker container ls --all
```

## Bajar HTML de Prueba (Hola Mundo)
```bash
wget https://raw.githubusercontent.com/DesarrolloEnGCP/DesarrolloEnGCP-Udemy/master/index.html
```

## Abrir HTML "Hola Mundo"
<walkthrough-editor-open-file filePath="./index.html"
                              text="Abrir Archivo de Prueba">
</walkthrough-editor-open-file>
