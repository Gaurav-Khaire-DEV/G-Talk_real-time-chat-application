# CDAC-Project
A real-time chat application developed using springboot

### BACKEND BUILD INSTRUCTIONS
docker run -d -p 6379:6379 redis:7

docker run -d -p 9000:9000 -p 9001:9001 -e "MINIO_ROOT_USER=admin" -e "MINIO_ROOT_PASSWORD=password" minio/minio server /data --console-address ":9001" 
curl -O https://dl.min.io/client/mc/release/linux-amd64/mc 
chmod +x mc 
Optional for Local (Avoid for EC2) (sudo mv mc /usr/local/bin/) 
./mc alias set myminio http://localhost:9000 admin password

docker run -d --name discord-mysql -p 3307:3306 -e "MYSQL_ROOT_PASSWORD=rootpassword" -e "MYSQL_USER=discord" -e "MYSQL_PASSWORD=discord" -e "MYSQL_DATABASE=discord_db" mysql:8

### TODOS
- [ ] Documentation
  - [ ] Backend Architecture
  - [ ] Use Case Diagrams & Sequence Diagram
- [ ] Reworking the Frontend
- [ ] Code cleaup on backend




# Discord Clone

A simple **Discord-like chat application** created for learning and demonstration purposes.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)

---

## Overview

This project is a **Real-Time Chat Application** that demonstrates:

- Client–server architecture
- Authentication and authorization concepts
- Real-time communication fundamentals
- Clean project structuring

It is intended for **educational use**, not production deployment.

---

## Features

- User authentication
- Channel-based messaging
- Real-time chat (WebSocket-based)
- REST APIs for non-real-time operations

---

## Tech Stack

### Backend
- Java
- Spring Boot
- Spring Security
- JPA / Hibernate

### Frontend
- React
- WebSocket / SockJS

### Tools
- Gradle
- MinIO
- Git
- Postman

---


