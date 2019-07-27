# Primeros Pasos con Cloud Shell y Docker.

## Comprobar version de Docker

```bash
docker --version
```

## Bajar y Ejecutar Imagen de Docker "Hola Mundo"
```bash
docker run hello-world
```

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
