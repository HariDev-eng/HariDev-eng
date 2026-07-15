<div align="center">

# Hi 👋 I'm Hari Pradap

### Backend Engineer • Distributed Systems Enthusiast • Microservices Builder

<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=22&duration=3500&pause=1000&center=true&vCenter=true&width=650&lines=Backend+Developer;Building+Distributed+Systems;Learning+Software+Architecture;Go+%7C+Spring+Boot+%7C+Kafka+%7C+RabbitMQ;Always+Building.+Always+Learning." />

</div>

---

## 🚀 About Me

I'm a backend developer passionate about building scalable systems and understanding **why** software is designed the way it is.

I recently graduated with a **B.Tech in Information Technology** and completed a **10-month internship at Marmin Technologies**, where I worked on:

- REST APIs
- Financial document workflows
- Webhook delivery systems
- RabbitMQ
- SaaS compliance platform
- PostgreSQL
- Go backend services

Today I'm focused on learning backend engineering by building **real distributed systems** instead of isolated tutorials.

My goal isn't just to write code.

It's to understand architecture, scalability, distributed systems, and the engineering trade-offs behind production software.

---

# 🚧 Currently Building

## 🏥 Distributed Patient Management Platform

A healthcare platform built from scratch using **microservices** and **event-driven architecture**.

### Current Progress

| Component | Status |
|-----------|---------|
| 🌐 React Frontend | 🚧 |
| 🚪 API Gateway | ✅ |
| 👤 Patient Service | ✅ |
| 👨‍⚕️ Doctor Service | ✅ |
| 🩺 Nurse Service | ✅ |
| 📅 Appointment Service | ✅ |
| 🧾 Diagnosis Service | ✅ |
| 📦 Inventory Service | ✅ |
| 🔔 Notification Service (Go) | 🚧 |
| 🔐 Authentication Service | 🚧 |
| 📨 Kafka Event Streaming | ✅ |
| 🐇 RabbitMQ Workers | 🚧 |
| 🔗 gRPC Communication | ✅ |
| 🐳 Docker | 🚧 |
| ☁ Kubernetes | 📅 Planned |

---

# 🏗 Architecture Snapshot

```text
                        React UI

                            │

                     API Gateway

                            │

────────────────────────────────────────────────────────

 Patient Service

 Doctor Service

 Nurse Service

 Appointment Service

 Diagnosis Service

 Inventory Service

 Notification Service (Go)

 Authentication Service

────────────────────────────────────────────────────────

 REST APIs

 gRPC

 Kafka

 RabbitMQ

────────────────────────────────────────────────────────

 PostgreSQL

 Redis

 Docker
```

---

## 🧠 What I'm Learning

Instead of building isolated CRUD applications, I'm currently exploring backend engineering through real projects.

Current focus:

- Distributed Systems
- Microservices
- Event-Driven Architecture
- CQRS
- Kafka
- RabbitMQ
- gRPC
- Software Architecture
- Domain-Driven Design
- SOLID Principles
- Clean Architecture
- Scalability
- System Design
- Cloud Native Development

---

## 🎯 Current Goal

Build a production-style healthcare platform that helps me understand:

- Designing scalable backend systems
- Service-to-service communication
- Distributed messaging
- Event-driven workflows
- Production architecture
- Cloud-native applications

Alongside the project, I'm documenting every major architectural decision to build my own **Backend Architecture Handbook**.

> *Learn by Building • Improve by Refactoring • Understand by Documenting*


# 🚀 Featured Projects

These are projects I've built to understand backend engineering, distributed systems, concurrency, and software architecture through real implementation.

---

# 🏥 Distributed Patient Management Platform

> **A production-style healthcare platform built with microservices, event-driven architecture, and distributed communication.**

This project is my primary learning platform for backend engineering. Rather than building isolated CRUD services, I'm designing a complete distributed system where each service owns its own responsibility, database, and communication patterns.

## 🏗 Architecture

```text
                    React Frontend
                          │
                          ▼
                    API Gateway
                          │
        ┌─────────────────┼──────────────────┐
        │                 │                  │
        ▼                 ▼                  ▼
 Patient Service     Doctor Service     Auth Service
        │                 │
        │                 ▼
        │         Appointment Service
        │                 │
        │                 ▼
        │         Diagnosis Service
        │
        ▼
 Notification Service (Go)

──────────────────────────────────────────────

REST APIs

gRPC

Apache Kafka

RabbitMQ

──────────────────────────────────────────────

PostgreSQL

Docker
```

---

## 📦 Microservices

| Service | Responsibility |
|----------|----------------|
| 🌐 API Gateway | Centralized routing and request forwarding |
| 👤 Patient Service | Patient registration and profile management |
| 👨‍⚕️ Doctor Service | Doctor profiles, availability and specialization |
| 🩺 Nurse Service | Nurse assignment and ward management |
| 📅 Appointment Service | Appointment scheduling and lifecycle |
| 🧾 Diagnosis Service | Medical diagnosis and patient history |
| 📦 Inventory Service | Medical inventory management |
| 🔔 Notification Service (Go) | Email, SMS and In-App notification processing |
| 🔐 Authentication Service | JWT authentication and authorization |

---

## ⚡ Communication Patterns

### REST APIs

Client communication and external service access.

### gRPC

High-performance synchronous communication between services.

Examples:

- Appointment → Patient Verification
- Appointment → Doctor Availability

---

### Apache Kafka

Used for asynchronous business events.

Current event flow:

```text
Appointment Created

        │

        ▼

Kafka

        │

        ▼

Notification Service

        │

        ▼

Notification Processing
```

---

### RabbitMQ

Used for asynchronous background workers.

```text
Notification

        │

        ▼

RabbitMQ

        │

        ▼

Email Worker

SMS Worker

In-App Worker
```

---

## 🧠 Concepts Implemented

- Microservices
- Event-Driven Architecture
- CQRS
- Event-Carried State Transfer
- RabbitMQ Workers
- Apache Kafka
- gRPC
- API Gateway
- JWT Authentication
- Protocol Buffers
- Repository Pattern
- Builder Pattern
- Factory Pattern
- Clean Architecture

---

## 🛠 Tech Stack

`Spring Boot`
`Go`
`React`
`PostgreSQL`
`Kafka`
`RabbitMQ`
`gRPC`
`Protocol Buffers`
`Docker`
`JWT`

---

### 🔗 Repositories

**Backend**

https://github.com/HariDev-eng/Patient-Management-System

**Frontend**

https://github.com/HariDev-eng/patient-management-ui

---

# 🎬 Concurrent Movie Seat Booking System

> Preventing double booking under heavy concurrency using multiple synchronization strategies.

A Go backend built to understand concurrency, synchronization, race conditions and distributed locking.

---

## Features

- Goroutines
- Mutex (sync.RWMutex)
- Redis Atomic SET NX
- Interface-driven storage implementations
- Concurrent load testing
- Benchmark comparison

---

## Implemented Strategies

✅ In-Memory

✅ Mutex Protected

✅ Redis Atomic Operations

---

## Tech Stack

`Go`
`Redis`
`Goroutines`
`REST APIs`
`Clean Architecture`

---

🔗 Repository

https://github.com/HariDev-eng/concurrent-movie-booking

---

# 🔗 Event-Driven Webhook Processing System

> A webhook platform inspired by Stripe, GitHub and modern SaaS products.

Built to understand asynchronous event delivery and reliable webhook processing.

---

## Features

- Event-driven processing
- RabbitMQ
- Retry mechanism
- Asynchronous workers
- Reliable webhook delivery
- Producer / Consumer architecture

---

## Tech Stack

`Go`
`RabbitMQ`
`REST APIs`
`Webhooks`

---

🔗 Repository

https://github.com/HariDev-eng/Event-Driven-Webhook-Processing-System

---

# 📝 Blog Platform

> A secure REST backend built with Spring Boot and Spring Security.

---

## Features

- JWT Authentication
- Spring Security
- Role-Based Access Control
- CRUD APIs
- Categories
- Tags
- PostgreSQL

---

## Tech Stack

`Spring Boot`
`Spring Security`
`JWT`
`PostgreSQL`

---

🔗 Repository

https://github.com/HariDev-eng/Blog-App

---

# 🚀 What's Next?

I'm currently expanding the Patient Management Platform with:

- ✅ Authentication Service
- ✅ Notification Service
- 🔄 Docker Deployment
- 🔄 Kubernetes
- 🔄 AWS
- 🔄 CI/CD
- 🔄 Observability
- 🔄 Distributed Tracing

The goal isn't simply to add technologies—it's to understand the engineering trade-offs involved in designing and evolving distributed backend systems.



# 🛠 Tech Stack

## 💻 Languages

<p>
  <img src="https://skillicons.dev/icons?i=go,java,javascript,python" />
</p>

---

## ⚙️ Backend

<p>
  <img src="https://skillicons.dev/icons?i=spring,nodejs" />
</p>

**Technologies**

- REST APIs
- gRPC
- Apache Kafka
- RabbitMQ
- Protocol Buffers
- JWT Authentication
- Spring Security
- Webhooks

---

## 🗄 Databases

<p>
  <img src="https://skillicons.dev/icons?i=postgres,mongodb,redis,mysql" />
</p>

---

## 🎨 Frontend

<p>
  <img src="https://skillicons.dev/icons?i=react,tailwind" />
</p>

---

## ☁ DevOps & Tools

<p>
  <img src="https://skillicons.dev/icons?i=docker,git,linux" />
</p>

Currently Learning:

- Kubernetes
- AWS
- CI/CD
- GitHub Actions
- Terraform

---

# 🧠 Engineering Journey

I believe the best way to learn software engineering is to build increasingly complex systems and continuously improve them.

Instead of collecting tutorials, I focus on building projects that force me to solve real engineering problems.

Over the past year I've gradually moved from building CRUD applications to designing distributed systems.

Current areas of focus:

- Backend Engineering
- Distributed Systems
- Event-Driven Architecture
- Software Architecture
- Cloud-Native Applications
- Microservices
- Scalability
- System Design

---

# 📚 Currently Learning

Rather than trying to learn everything at once, I'm progressing one topic at a time.

## Backend

- ✅ REST APIs
- ✅ Spring Boot
- ✅ Go
- ✅ gRPC
- ✅ Kafka
- ✅ RabbitMQ
- 🔄 Authentication & Authorization
- 🔄 Docker
- 🔄 Kubernetes
- 🔄 AWS

---

## Software Architecture

- ✅ SOLID Principles
- ✅ Clean Architecture
- 🔄 Domain-Driven Design
- 🔄 CQRS
- 🔄 Event-Driven Architecture
- 🔄 Event-Carried State Transfer
- 🔄 Distributed Messaging
- 🔄 Architectural Decision Records (ADRs)

---

## Distributed Systems

- Kafka
- RabbitMQ
- Retry Strategies
- Dead Letter Queues
- Transactional Outbox
- Idempotency
- Eventual Consistency
- Distributed Transactions

---

# 🎯 2026 Goals

- ✅ Build a distributed healthcare platform
- 🔄 Deploy every service with Docker
- 🔄 Learn Kubernetes
- 🔄 Learn AWS
- 🔄 Build CI/CD pipelines
- 🔄 Build a Backend Architecture Handbook
- 🔄 Contribute to Open Source
- 🔄 Land a Backend Engineer role

---

# 💡 Engineering Philosophy

> "Learn by building.
>
> Improve by refactoring.
>
> Understand by documenting."

Every project I build starts simple.

As I encounter new problems, I study the trade-offs, redesign the architecture, document the decision, and continue improving.

That process has taught me far more than simply following tutorials.

---

# 📈 Current Learning Roadmap

```text
Backend Development
        │
        ▼
Microservices
        │
        ▼
Event-Driven Systems
        │
        ▼
Distributed Systems
        │
        ▼
Software Architecture
        │
        ▼
Cloud Native Engineering
        │
        ▼
Platform Engineering
```

---

# 🌱 Beyond Code

When I'm not coding, you'll usually find me:

🏋️ Working out

📚 Reading about distributed systems and software architecture

📝 Documenting what I learn

🧩 Solving algorithmic problems

🚀 Building side projects to experiment with new ideas

---

# 📖 What You'll Find on My GitHub

✔ Production-style backend projects

✔ Microservices

✔ Event-driven architectures

✔ Distributed systems experiments

✔ Concurrency projects

✔ Backend learning notes

✔ Architecture Decision Records (ADRs)

✔ Real-world engineering experiments

Instead of uploading dozens of unfinished repositories, I prefer building a few projects deeply and continuously improving them.


---

# 📊 GitHub Analytics

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=HariDev-eng&show_icons=true&theme=transparent&hide_border=true&rank_icon=github"/>

<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=HariDev-eng&layout=compact&theme=transparent&hide_border=true"/>

</div>

---

<div align="center">

<img src="https://streak-stats.demolab.com?user=HariDev-eng&theme=transparent&hide_border=true"/>

</div>

---

# 🏆 GitHub Activity

<div align="center">

<img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=HariDev-eng&theme=github"/>

</div>

---

# 📈 Contributions

<div align="center">

<img src="https://github-readme-activity-graph.vercel.app/graph?username=HariDev-eng&theme=github-compact&hide_border=true"/>

</div>

---

# 🎯 Current Focus

Currently working on building a distributed healthcare platform while learning:

- Backend Engineering
- Distributed Systems
- Event-Driven Architecture
- Cloud Native Applications
- Software Architecture
- System Design

Current priorities:

```

🏥 Patient Management Platform

🔔 Notification Service

🔐 Authentication Service

🐳 Docker Deployment

☸ Kubernetes

☁ AWS
