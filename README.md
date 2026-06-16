# Hey, I'm Hari Pradap 👋

Backend developer who enjoys building systems that scale — microservices, distributed backends, and event-driven architectures. I recently graduated with a B.Tech in Information Technology and completed a 10-month internship at **Marmin Technologies**, where I worked on a SaaS-based compliance platform building APIs, financial document workflows, webhook delivery systems, and async communication using RabbitMQ.

I learn by building. Most of what's on this profile is me figuring things out by actually writing the code.

---

## 🛠 Tech I work with

**Languages**
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat&logo=go&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)

**Backend**
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=spring-boot&logoColor=white)
![Apache Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat&logo=apache-kafka&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=flat&logo=rabbitmq&logoColor=white)
![gRPC](https://img.shields.io/badge/gRPC-4285F4?style=flat&logo=google&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=node.js&logoColor=white)
![Webhooks](https://img.shields.io/badge/Webhooks-FF6B6B?style=flat&logo=zapier&logoColor=white)

**Databases**
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=flat&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-005C84?style=flat&logo=mysql&logoColor=white)

**Frontend**
![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white)

**Tools & DevOps**
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![Cypress](https://img.shields.io/badge/Cypress-17202C?style=flat&logo=cypress&logoColor=white)

---

## 🚀 Projects I'm proud of

### 🏥 Patient Management System — Full Stack Microservices

A production-grade microservices platform built with Spring Boot, featuring a full React UI, API Gateway, and 8 independently deployable services.

**Services:**
| Service | Responsibility |
|---|---|
| `patient-service` | Patient registration, records, profile management |
| `doctor-service` | Doctor profiles, availability, specialization |
| `nurse-service` | Nurse assignments and ward management |
| `appointment-service` | Booking, scheduling, status tracking |
| `diagnosis-service` | Patient diagnosis records and history |
| `inventory-service` | Medical inventory and stock management |
| `auth-service` | JWT-based authentication and authorization |
| `api-gateway` | Centralized routing, JWT validation, load balancing |

**Communication patterns:**
- **gRPC** — synchronous inter-service calls with Protocol Buffer contracts (e.g. Appointment → Patient verification)
- **Kafka** — async event streaming for billing creation, notifications, and audit logs
- **Proto files** — shared contract definitions across all services

**UI:** React + Tailwind CSS frontend (separate repository) — 50% complete, actively in development

**Repos:**
[Backend Services](https://github.com/HariDev-eng/Patient-Management-System) · [Frontend UI](https://github.com/HariDev-eng/patient-management-ui)

`Spring Boot` `Kafka` `gRPC` `Docker` `PostgreSQL` `React` `JWT` `Protocol Buffers`

---

### 🎬 [Concurrent Movie Seat Booking System](https://github.com/HariDev-eng/concurrent-movie-booking)

A Go backend built to solve the hard problem of concurrent seat booking — preventing double-booking under 100,000 simultaneous requests. Implemented three storage strategies: in-memory, mutex-protected (sync.RWMutex), and Redis-backed with atomic SET NX operations.

Benchmarked all three strategies for throughput and correctness under load. Clean architecture with interface-based pluggable storage backends.

`Go` `Redis` `Goroutines` `Clean Architecture` `REST APIs`

---

### 📝 [Blog Platform](https://github.com/HariDev-eng/Blog-App)

A Spring Boot blog backend with JWT authentication, role-based access control via Spring Security, and full CRUD for posts, categories, and tags on PostgreSQL. Normalized schema design with proper indexing for query performance.

`Spring Boot` `Spring Security` `JWT` `PostgreSQL` `REST APIs`

---

### 🔗 [Event-Driven Webhook Processing System](https://github.com/HariDev-eng/Event-Driven-Webhook-Processing-System)

A Go-based webhook processing system built around event-driven principles — reliable delivery, retry logic, and async processing pipelines.

`Go` `Webhooks` `Event-Driven` `RabbitMQ`

---

## 📊 GitHub Stats

![](https://github-profile-summary-cards.vercel.app/api/cards/stats?username=HariDev-eng&theme=default)
![](https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=HariDev-eng&theme=default)

![GitHub Streak](https://streak-stats.demolab.com?user=HariDev-eng&theme=default&hide_border=true)

---

## 📬 Let's connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/hari-pradap-490663260)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:haripradap09@gmail.com)

---

*Currently open to backend and full-stack roles. If you're building something interesting, let's talk.*
