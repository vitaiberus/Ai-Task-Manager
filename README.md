# 🚀 Backend Technologies

This project is built using a modern **Java & Spring ecosystem**, following a **microservices architecture** with secure communication, event-driven processing, caching, and AI integration.

## 🛠️ Technology Stack

| Technology                  | Purpose                                                                                   |
| --------------------------- | ----------------------------------------------------------------------------------------- |
| ☕ **Java**                  | Core programming language used to build backend services.                                 |
| 🍃 **Spring Boot**          | Builds production-ready microservices quickly with minimal configuration.                 |
| ☁️ **Spring Cloud**         | Provides tools for service discovery, centralized configuration, and distributed systems. |
| 🔐 **Spring Security**      | Handles authentication, authorization, and application security.                          |
| 🗄️ **Spring Data JPA**     | Simplifies database access and persistence using Java entities and repositories.          |
| 🚪 **Spring Cloud Gateway** | Acts as a single entry point for API routing, filtering, and security.                    |
| 🔗 **OpenFeign**            | Enables simple and declarative service-to-service communication.                          |
| 🛡️ **Resilience4j**        | Provides circuit breakers, retries, rate limiting, and fault tolerance.                   |
| 🔑 **JJWT**                 | Creates, signs, and validates JWT tokens for secure API authentication.                   |
| 📨 **Apache Kafka**         | Enables asynchronous communication and event-driven architecture.                         |
| ⚡ **Redis**                 | Provides high-performance caching and fast data access.                                   |
| 🐘 **PostgreSQL**           | Stores structured relational data with strong consistency and reliability.                |
| 🤖 **Google GenAI SDK**     | Integrates Google Gemini AI capabilities into backend services.                           |
| ✉️ **Spring Boot Mail**     | Sends transactional emails through SMTP providers.                                        |
| 🧩 **Lombok**               | Reduces boilerplate Java code such as getters, setters, and constructors.                 |
| 📦 **Apache Maven**         | Manages project dependencies, builds, and the application lifecycle.                      |

---

## 🏗️ Architecture

The backend follows a **microservices and event-driven architecture**.

```text
                         ┌─────────────────┐
                         │      Users      │
                         └────────┬────────┘
                                  │
                                  ▼
                         ┌─────────────────┐
                         │   API Gateway   │
                         │  Spring Cloud   │
                         └────────┬────────┘
                                  │
                    ┌─────────────┼─────────────┐
                    ▼             ▼             ▼
              ┌───────────┐ ┌───────────┐ ┌───────────┐
              │ Service A │ │ Service B │ │ Service C │
              │Spring Boot│ │Spring Boot│ │Spring Boot│
              └─────┬─────┘ └─────┬─────┘ └─────┬─────┘
                    │             │             │
                    ▼             ▼             ▼
              ┌─────────────────────────────────────┐
              │      PostgreSQL / Redis Storage     │
              └──────────────────┬──────────────────┘
                                 │
                                 ▼
                       ┌───────────────────┐
                       │   Apache Kafka    │
                       │  Event Streaming  │
                       └─────────┬─────────┘
                                 │
                    ┌────────────┴────────────┐
                    ▼                         ▼
             ┌──────────────┐          ┌──────────────┐
             │  Analytics   │          │ Gemini AI    │
             └──────────────┘          └──────────────┘
```

### 🔄 Application Flow

**Users** → **API Gateway** → **Microservices** → **PostgreSQL / Redis** → **Apache Kafka** → **Analytics & AI**

---

## 🔐 Security

The application uses:

* **Spring Security** for authentication and authorization
* **JWT (JJWT)** for stateless API authentication
* **Spring Cloud Gateway** for centralized request filtering and security
* **Resilience4j** for fault tolerance and service resilience

## 📡 Communication

The microservices communicate using two approaches:

* **OpenFeign** — synchronous service-to-service communication
* **Apache Kafka** — asynchronous event-driven communication

## 🤖 AI Integration

**Google GenAI SDK** provides integration with **Google Gemini**, allowing backend services to use generative AI capabilities for intelligent application features.

---

### Backend Stack

`Java` • `Spring Boot` • `Spring Cloud` • `Spring Security` • `Spring Data JPA` • `Spring Cloud Gateway` • `OpenFeign` • `Resilience4j` • `JJWT` • `Apache Kafka` • `Redis` • `PostgreSQL` • `Google GenAI SDK` • `Spring Boot Mail` • `Lombok` • `Maven`
