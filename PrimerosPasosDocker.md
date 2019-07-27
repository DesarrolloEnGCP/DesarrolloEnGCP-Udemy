# Primeros Pasos con Cloud Shell y Docker.

## Comprobar version de Docker

```bash
docker --version
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

## Abrir HTML "Hola Mundo"
<walkthrough-editor-open-file filePath="./DesarrolloEnGCP-Udemy/index.html"
                              text="Abrir Archivo de Prueba">
</walkthrough-editor-open-file>
