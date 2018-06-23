# Demo Servidor Redis

Introducción al servidor redis

# Requisitos

1. Asumo que has leido la documentacion de redis https://redis.io/

2. El servidor de redis está dockerizado, es necesario tener docker y docker-compose instalado. Info para la instalación: https://gitlab.com/snippets/1722766 o google ;)

3. Cliente de redis **redis-cli** (ejecuta el siguiente comando para instalarlo, suponiendo que estes en ubuntu/debian)
```
sudo apt-get install redis-tools
```

# Servidor de redis

## Arrancar el servidor de redis

Escribe en el terminal:
```
docker-compose up --build
```

## Parar el servidor de redis

* Opción 1: Pulsta Ctrl+C en el terminal donde has arrancado el servidor redis

* Opción 2: Abre un terminal y escribe: 
```
docker stop demoredis_redis-server_1
```
Nota el nombre del contenedor puede ser distinto si has modificado el fichero docker-compose.yml

## Cliente **redis-cli**

En un terminal escribe:
```
redis-cli
```
Una vez conectado al servidor de redis, ya puedes provar los comandos explicados en https://redis.io/commands

Para salir del cliente, escribe "exit"

