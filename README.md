# Nginx-Docker
Prueba de Nginx sirviendo contenido HTML estático desde un contenedor de Docker

## Correr Nginx en un contenedor de Docker

### Correr el contenedor con docker-compose con el siguiente comando
```bash
# Iniciar el contenedor con docker desde el archivo docker-compose.yml
$ docker-compose up
```
```bash
# Detener el contenedor con docker compose
$ docker-compose stop
```
```bash
# Eliminar el contenedor con docker compose
$ docker-compose rm
```

### O correr el contenedor desde la terminal con el siguiente comando
```bash
# Iniciar el contenedor con comando docker
$ docker run --name my-nginx -p 8080:80 -v ./html:/usr/share/nginx/html:ro nginx:1.25-alpine
```
```bash
# Detener el contenedor con comando docker
$ docker stop <id o nombre del contenedor>
```

```bash
# Eliminar el contenedor con comando docker
$ docker rm <id o nombre del contenedor>
```

### Fuente
[Imagen docker oficial de Nginx](https://hub.docker.com/_/nginx)

## Subir los cambios al repositorio

### Comandos Git
```bash
# Agrega los cambios de todos los archivos para el próximo commit

git add .
```

```bash
# Crea un nuevo commit con un mensaje descriptivo

git commit -m "Agregados los archivos index.html y docker-compose.yml con imagen de Nginx"
```

```bash
# Envía los cambios del commit al repositorio remoto

git push
```
