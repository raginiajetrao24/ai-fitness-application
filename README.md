# AI-Powered Fitness Activity Recommendation System

A microservices-based fitness tracking application that enables users to log activities and receive AI-powered personalized fitness recommendations.

---

## 📌 Project Overview

This application allows users to:

- Log fitness activities (activity type, duration, calories burned)
- Store both structured and flexible activity data
- Generate AI-based personalized fitness recommendations
- Experience a scalable and secure microservices backend architecture

The system follows modern backend design principles including centralized configuration, service discovery, secure authentication, and asynchronous communication.

---

## 🏗 Architecture

The project follows a distributed microservices architecture consisting of:

- Config Server (Centralized Configuration Management)
- Eureka Server (Service Discovery)
- API Gateway (Centralized Routing & Security)
- User Service
- Activity Service
- AI Service

---

## 🔧 Architectural Highlights

- **Spring Boot** for independent backend services
- **Spring Cloud Config Server** for centralized configuration management
- **Eureka Server** for service registration and discovery
- **Spring Cloud Gateway** for centralized routing
- **Keycloak** for authentication and role-based access control
- **RabbitMQ** for asynchronous inter-service communication
- **MySQL** for structured relational data
- **MongoDB** for flexible activity logs and AI recommendation storage
- **Google Gemini API** for AI-powered fitness insights

---

## 🛠 Tech Stack

### Backend
- Java
- Spring Boot
- Spring Data JPA
- Hibernate
- Microservices Architecture

### Configuration & Discovery
- Spring Cloud Config Server
- Eureka Server

### Communication
- RabbitMQ (Asynchronous Messaging)

### Databases
- MySQL (Relational Data)
- MongoDB (Flexible Activity & AI Data)

### API & Security
- RESTful APIs
- API Gateway
- Keycloak Authentication

### AI Integration
- Google Gemini API

---

## 🚀 Key Features

- Centralized configuration management using Config Server
- Service discovery using Eureka
- Secure authentication via Keycloak integrated with API Gateway
- Activity logging with structured (MySQL) and flexible (MongoDB) storage
- AI-generated personalized fitness recommendations
- Asynchronous communication using RabbitMQ
- Scalable and modular microservices design

---

## 🔄 Data Flow (High-Level)

1. User authenticates via Keycloak through API Gateway.
2. User logs fitness activity.
3. Activity data stored in MySQL.
4. Flexible activity logs stored in MongoDB.
5. RabbitMQ triggers AI Service.
6. Gemini API generates personalized fitness insights.
7. Recommendations stored in MongoDB.
8. Response returned through API Gateway.

---

## ▶️ How to Run the Project

Ensure the following services and components are properly configured and running:

### 🔹 Infrastructure Services
1. Start Config Server (centralized configuration).
2. Start Eureka Server (service registry).

### 🔹 Security Setup
3. Start Keycloak server.
   - Create realm.
   - Configure client for API Gateway.
   - Set up user roles and credentials.

### 🔹 Core Microservices
4. Start User Service.
5. Start Activity Service.
6. Start AI Service.

### 🔹 API Gateway
7. Start API Gateway (integrated with Keycloak for authentication and routing).

### 🔹 External Dependencies
8. Ensure RabbitMQ is running.
9. Ensure MySQL and MongoDB are running.

### 🔹 Frontend
10. Run the frontend application.

---

## 📈 Future Improvements

- Add caching using Redis
- Implement centralized logging
- Containerize services using Docker
- Deploy using Kubernetes
- Enhance AI recommendation personalization

---

## 👩‍💻 Developed By

Ragini Ajetrao  
CDAC PG-DAC  
Full Stack & Backend Developer
