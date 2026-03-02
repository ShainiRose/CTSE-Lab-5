# Microservices System - CTSE Lab 5

This repository contains a complete microservices system with:
- API Gateway
- Item Service
- Order Service
- Payment Service

## Tech Stack
- Java 21
- Spring Boot
- Maven
- Docker + Docker Compose

## Project Structure
- `api-gateway/`
- `itemservice/`
- `orderservice/`
- `paymentservice/`
- `docker-compose.yml`

## Prerequisites
- Java 21
- Maven (or use `mvnw` in each service)
- Docker Desktop (running)

## Build JAR Files
Run these commands from the project root:

```powershell
cd itemservice
.\mvnw.cmd clean package

cd ..\orderservice
.\mvnw.cmd clean package

cd ..\paymentservice
.\mvnw.cmd clean package

cd ..\api-gateway
.\mvnw.cmd clean package
```

## Run with Docker
From the project root:

```powershell
docker compose up --build -d
```

Check running containers:

```powershell
docker compose ps
```

Stop all services:

```powershell
docker compose down
```

## Service Ports
- API Gateway: `http://localhost:8080`
- Item Service: `http://localhost:8081`
- Order Service: `http://localhost:8082`
- Payment Service: `http://localhost:8083`





