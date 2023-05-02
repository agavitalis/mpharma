# mPharma Microservices with RabbitMQ 
mPharma Diagnosis Microservices quick app using **NestJS / RabbitMQ**.

## Dependencies & Services
- RabbitMQ - https://www.rabbitmq.com
- Redis - https://redis.io
- PostgreSQL - https://www.postgresql.org
- TypeORM - https://typeorm.io


## Get started Notes:
- Use `git submodule update --init --recursive` command to update/fetch submodules.
- Update `.env` file with the necessary credentials 
- Diagnosis-service endpoint: `host:port/api/health`
- Notification-service endpoint: `host:port/api/docs`

## Run in local(Individual service)

To start diagnosis-service folder `cd diagnosis-service`
```bash
npm install
npm run start:dev
```

To start notification-service folder `cd notification-service`
```bash
npm install
npm run start:dev
```

## Run Local Env in docker-compose 
```bash
docker-compose up
```
## Docker Notes:
- Use `name` of the service to connect service internally with docker compose environment.
- for rebuild services use command `docker-compose up --build`.  

# To access diagnosis-service : http://192.168.49.2:30353

# To access notification-service : http://192.168.49.2:30353

