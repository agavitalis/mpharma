# # mPharma Notification-Service API

This project is the notification service of mPharma application

## Prerequisites
- Node.js 
- Yarn or NPM
- MongoDB
- RabbitMQ


## Installation
- Install dependencies with yarm
```bash
yarn install 
```
- Install dependencies with npm
```bash
npm install 
```
## Running the app

- Create local environment file and update the env variables
```shell
cp .env.example .env
nano .env
```
- Start Application in development mode 
```bash
npm run start:dev
```
The application will be live on http://localhost:5002

- Start Application in production mode
```bash
npm run build
```

```bash
npm run start:dev
```

The application will be live on http://localhost:5002 
## Running the app with docker

You can also run this application using docker by building the image and mapping the necessary ports. This process requires that you have docker pre-installed in your system.
 
To proceed,navigate to the root directory of the application and build the application image using the following command:

```bash
docker build . -t <your username>/customer-service
```
Run your image in detached mode with -d tag. The -p flag map a public port to a private port inside the container. Run the image you previously built using the command:

```bash
docker run -p 5002:5002 -d <your username>/customer-service
```

The application will be live on http://localhost:5002

## Stay in touch

- Author - [Ogbonna Vitalis](agavitalisogbonna@gmail.com)

## License

Licence is [MIT licensed](LICENSE).
