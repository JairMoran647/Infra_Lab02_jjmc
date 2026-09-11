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

Variable de entorno hecho con un mensaje unico de Moran Carbonel Jair Compilado 


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
#  Responder los tipos de redes y los tipos de volumen que existen en docker

Los tipos de redes y los tipos de volumenes que existen en docker son:
  
  Bridge: El cual es una red usada por defecto en Docker cuando se crean contenedores de una mismo host

  Host: El contenedor usa directamente la red del equipo anfitrion, no existe una separacion entre los puertos del contenedor y los puertos del SO

  None: Deshabilita completamente la comunicacion de red del contenedor, el contenedor queda aislado y no puede comunicarse con los otros servicios

  Overlay: Nos permite conectar contenedores ubicados en diferentes maquinas Docker el cual utiliza principalmente en ambientes con Docker Swarm para trabajar con aplicaciones distribuidas

  *Volumenes en Docker: Los volumenes permiten almacenar informacion fuera del ciclo de vida del contenedor, esto para evitar perder datos cuando un contenedor es eliminado
    *Volumen nombrado: Es un volumen administrado completamente por Docker y tiene un nombre especifico

  En este proyecto usamos por ejemplo:
  - postgrades_data:/var/lib/postgresql/data
  En el docker-compose

# Creditos
- Moran Carbonel Jair Jesus
ID 000284492

# ETC


# Imagenes 

Crearemos una carpeta para las capturas que evidencian mi trabajo

la cual se llama capturas

Gracias por su atencion .
