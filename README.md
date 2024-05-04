# Running Microservices with Docker Compose

This repository contains Dockerfiles and a docker-compose.yml file to build and run the demo microservices along with PostgreSQL 10.

## Prerequisites

- Docker
- Docker Compose

## Steps to Run the Application

1. Clone this repository:
```
git clone https://github.com/HamzaSusic basic-microservices-docker.git

```

2. Navigate to the cloned directory:
```
    cd basic-microservices-docker
```
3. Run the following command to start the application along with PostgreSQL:
```
    docker-compose up --build
```
4. Once all services are running, execute the following command locally to verify the health status:
```
    bash <(curl -s https://raw.githubusercontent.com/kkenan/basic-microservices/master/health_check.sh)
```
5. If all checks pass, you should see the output: "All checks passed. Congrats!"

6. Access the Spring Boot App at http://localhost:8080 and the Node.js App at http://localhost:8081.


7. To stop the application, press `Ctrl + C` in the terminal where `docker-compose up` is running.

