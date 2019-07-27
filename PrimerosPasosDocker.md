# Primeros Pasos con Cloud Shell y Docker.

## Comprobar version de Docker

```bash
docker --version
```
### Para limpiar todo y comenzar desde cero (si intentaste este tutorial antes) ejecuta este comando:
```bash
docker system prune -a
```


## Bajar y Ejecutar Imagen de Docker "Hola Mundo"
```bash
docker run hello-world
```
**SALIDA**
Unable to find image 'hello-world:latest' locally
latest: Pulling from library/hello-world
1b930d010525: Pull complete
Digest: sha256:6540fc08ee6e6b7b63468dc3317e3303aae178cb8a45ed3123180328bcc1d20f
Status: Downloaded newer image for hello-world:latest

Hello from Docker!
This message shows that your installation appears to be working correctly.

## Ver Imagenes Descargadas (la del paso anterior)
```bash
docker image ls
```

## Ver Contenedores (el modificar "--all" incluye los contenedores finalizados)
```bash
docker container ls --all
```

## Abrir HTML "Hola Mundo" (y modificar)
<walkthrough-editor-open-file filePath="./DesarrolloEnGCP-Udemy/index.html"
                              text="Abrir Archivo de Prueba">
</walkthrough-editor-open-file>

## Ejecutar un contenedor Web (nombre: hola-web)

Usaremos la imagen ofician de NGIX (Servidor Web*) desde el repositorio oficial de DockerHub: https://hub.docker.com/_/nginx

```bash
docker run --name hola-web -p 8080:80 -v $(pwd):/usr/share/nginx/html:ro -d nginx
```

## Navegar en nuestro sitio web (hola-mundo)
<walkthrough-spotlight-pointer spotlightId="devshell-web-preview-button"
                               text="Abrir navegador Web en puerto 8080">
</walkthrough-spotlight-pointer>

## Ver Contenedores (solo los en ejecución)
```bash
docker container ls
```

## Ver Imagenes Descargadas (ahora tenemos dos)
```bash
docker image ls
```

## Detener el contenedor (hola-web)
```bash
docker stop hola-web
```







