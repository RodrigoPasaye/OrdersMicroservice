# Orders Microservices

```
docker compose up -d
```

## Development pasos

1. Clonar el proyecto
2. Crear un archivo `.env` basado en el archivo `.env.template`
3. Ejecutar migración de prisma `npx prisma migrate dev`
4. Levantar la base de datos con `docker compose up -d`
5. Levantar el servidor de NATS

```
docker run -d --name nats-server -p 4222:4222 -p 8222:8222 nats
```

6. Levantar el proyecto con `npm run start:dev`
