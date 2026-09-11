# Laboratorio 02

Hoy utilizaremos docker compose para poder desplegar su trabajo. Servicio web y una base de datos

## Stack
API
  - Minimal API
    - Debe retornar un mensaje incluyendo mi nombre
  - Docker
  - Creacion de Dockers API 1, 2 y 3 con su respectivo ID y nombre
6b218b1c2930   postgres:13               "docker-entrypoint.s…"   36 seconds ago   Up 28 seconds   5432/tcp                                      lab02jjmc-db-1
1abe7c15739e   nmatsui/hello-world-api   "/sbin/tini -- npm s…"   37 seconds ago   Up 27 seconds   0.0.0.0:3000->3000/tcp, [::]:3000->3000/tcp   api01
0e384683b261   nmatsui/hello-world-api   "/sbin/tini -- npm s…"   37 seconds ago   Up 28 seconds   0.0.0.0:3002->3000/tcp, [::]:3002->3000/tcp   api03
07ef5200cd39   nmatsui/hello-world-api   "/sbin/tini -- npm s…"   37 seconds ago   Up 29 seconds   0.0.0.0:3001->3000/tcp, [::]:3001->3000/tcp   api02
 
*Hechos de forma manual* y luego automatizado con un docker-composer 

BD
  - PostgreSQL
- $ docker run --name some-postgres -e POSTGRES_PASSWORD=mysecretpassword -d postgres


# Indicaciones

## Comandos

```bash
docker compose up -d
```
Entornos 
Variables

```Inicializacion del API con
docker pull nmatsui/hello-world-api
```

```
Use docker compose down y docker compose up --build en muchas ocasiones para hacer cambios en el docker-compose y hacer pruebas con cambios neceasrios
```
## Configuración por entorno

```
MESSAGE=Jair Moran Carbonel
```


# Creditos
- Moran Carbonel Jair Jesus
ID 000284492

# ETC


# Imagenes 




