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

# 🎨 Frontend Technologies

The frontend is built with a modern **React ecosystem**, focusing on performance, scalability, responsive design, and a clean user experience.

### 🛠️ Technology Stack

| Technology             | Purpose                                                                              |
| ---------------------- | ------------------------------------------------------------------------------------ |
| ⚛️ **React**           | Builds dynamic, interactive, and component-based user interfaces.                    |
| ⚡ **Vite**             | Provides a fast development server and optimized production build system.            |
| 🗃️ **Redux Toolkit**  | Manages global application state efficiently with simplified Redux logic.            |
| 🔄 **React Redux**     | Connects React components with the Redux store.                                      |
| 🧭 **React Router**    | Handles client-side navigation and routing in the Single Page Application (SPA).     |
| 🌐 **Axios**           | Handles HTTP requests and communication between the frontend and backend APIs.       |
| 📝 **React Hook Form** | Manages form state and validation with high performance and minimal re-renders.      |
| ✅ **Zod**              | Provides schema-based validation for forms and API data.                             |
| 🎨 **Tailwind CSS**    | Enables fast and responsive UI styling using utility-first CSS classes.              |
| 🧩 **shadcn/ui**       | Provides modern, customizable, and reusable UI components.                           |
| ♿ **Radix UI**         | Provides accessible and unstyled UI primitives for building high-quality interfaces. |
| ✨ **Lucide**           | Supplies clean, lightweight, and customizable icons.                                 |
| 📅 **date-fns**        | Handles date formatting, parsing, and manipulation.                                  |

---

## ✨ Frontend Highlights

### ⚡ Fast Development

Built with **Vite** for a fast development experience, instant updates, and optimized production builds.

### 🚀 High Performance

Designed to minimize unnecessary rendering and provide a fast, smooth user experience.

### 📱 Responsive UI

The interface is designed to work seamlessly across:

**Desktop** • **Tablet** • **Mobile**

### 🧩 Scalable & Maintainable

The frontend follows a clean, modular architecture with reusable components, centralized state management, and clear separation of responsibilities.

---

## 🔄 Frontend Flow

```text
┌───────────────────┐
│       User        │
└─────────┬─────────┘
          │
          ▼
┌───────────────────┐
│     React UI      │
│ Tailwind + shadcn │
└─────────┬─────────┘
          │
          ├──────────────► React Router
          │
          ├──────────────► Redux Toolkit
          │
          └──────────────► Forms + Zod
          │
          ▼
┌───────────────────┐
│       Axios       │
└─────────┬─────────┘
          │
          ▼
┌───────────────────┐
│    API Gateway    │
└─────────┬─────────┘
          │
          ▼
┌───────────────────┐
│ Backend Services  │
└───────────────────┘
```

### Frontend Stack

`React` • `Vite` • `Redux Toolkit` • `React Redux` • `React Router` • `Axios` • `React Hook Form` • `Zod` • `Tailwind CSS` • `shadcn/ui` • `Radix UI` • `Lucide` • `date-fns`

# 🐳 Infrastructure & DevOps

The project uses modern **containerization, service discovery, centralized configuration, and event-driven infrastructure** to provide a scalable and reliable environment for microservices.

### 🛠️ Infrastructure Stack

| Technology                 | Purpose                                                                             |
| -------------------------- | ----------------------------------------------------------------------------------- |
| 🐳 **Docker**              | Packages applications and their dependencies into portable and isolated containers. |
| 📦 **Docker Compose**      | Runs and manages multiple application services with a single command.               |
| 🔍 **Eureka**              | Provides dynamic service registration and discovery between microservices.          |
| ⚙️ **Spring Cloud Config** | Centralizes configuration management across all microservices.                      |
| 📨 **Apache Kafka**        | Provides event streaming and asynchronous messaging for real-time data pipelines.   |

---

## 🚀 Infrastructure Highlights

### 📈 Scalable

Microservices can be scaled independently based on application load and demand.

### 🛡️ Reliable

Designed for high availability, resilience, and fault tolerance across distributed services.

### ⚡ Fast Deployment

Containerized services simplify application builds, deployment, and environment setup.

### 📊 Observability

Designed to support monitoring, logging, and tracking of overall system health and service performance.

### 🔐 Secure

Security is considered across the entire architecture, from the API Gateway to individual backend services.

---

## 🏗️ Infrastructure Architecture

```text
                         ┌─────────────────┐
                         │      Users      │
                         └────────┬────────┘
                                  │
                                  ▼
                         ┌─────────────────┐
                         │   API Gateway   │
                         └────────┬────────┘
                                  │
                 ┌────────────────┼────────────────┐
                 ▼                ▼                ▼
          ┌─────────────┐  ┌─────────────┐  ┌─────────────┐
          │  Service A  │  │  Service B  │  │  Service C  │
          │   Docker    │  │   Docker    │  │   Docker    │
          └──────┬──────┘  └──────┬──────┘  └──────┬──────┘
                 │                │                │
                 └────────────────┼────────────────┘
                                  │
                ┌─────────────────┼─────────────────┐
                ▼                 ▼                 ▼
         ┌────────────┐    ┌────────────┐    ┌────────────┐
         │ PostgreSQL │    │   Redis    │    │   Kafka    │
         └────────────┘    └────────────┘    └────────────┘

              Service Discovery → Eureka
              Configuration     → Spring Cloud Config
              Orchestration     → Docker Compose
```

### Infrastructure Stack

`Docker` • `Docker Compose` • `Eureka` • `Spring Cloud Config` • `Apache Kafka`


