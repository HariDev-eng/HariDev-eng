<div align="center">

<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=26&duration=3000&pause=1200&color=2E9EF7&center=true&vCenter=true&width=700&lines=Hi%2C+I'm+Hari+Pradap+%F0%9F%91%8B;Backend+Engineer;Distributed+Systems+%2B+Applied+AI;Go+%7C+Spring+Boot+%7C+Kafka+%7C+Kubernetes" alt="Typing SVG" />

[![GitHub](https://img.shields.io/badge/GitHub-HariDev--eng-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/HariDev-eng)
![Focus](https://img.shields.io/badge/Focus-Distributed%20Systems%20%2B%20Applied%20AI-2E9EF7?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Open%20to%20Backend%20Roles-brightgreen?style=for-the-badge)

</div>

<br>

## 🚀 About Me

I'm a backend engineer who builds distributed systems and cares about **why** software is designed the way it is.

I hold a **B.Tech in Information Technology** and completed a **10-month internship at Marmin Technologies**, where I owned a microservice end to end — 15 REST APIs, webhooks, RabbitMQ queues, and the database design — serving **1 lakh+ requests/day** on a live SaaS platform, and wrote **300+ automated Cypress tests** that caught 50+ bugs before release.

Since then I've been building larger systems on my own: an AI incident-analysis platform in Go, an 11-microservice healthcare platform deployed on Kubernetes with Jenkins, and a GraphQL ticketing system with an SLA engine. I work mainly in **Go** and **Java / Spring Boot**.

> *Learn by Building • Improve by Refactoring • Understand by Documenting*

<br>

## ⭐ Flagship Projects

### 🧭 OpsPilot — AI Incident Intelligence & Response Platform

An event-driven platform that ingests production events, groups them into incidents, and uses **RAG + LLMs** to produce evidence-backed root-cause analysis — with a human approving any action before it runs.

```
Events → Go API → PostgreSQL (events + outbox) → Kafka → Idempotent consumers
                                                         ↓
                                    Redis (incident state, dedup) → Incident engine
                                                         ↓
                          RAG (runbooks + past incidents) → LLM → Root-cause analysis
                                                         ↓
                                             Human approval → Action
```

- **Reliable ingestion:** `POST /api/v1/events` returns `202 Accepted` after saving the event and an outbox row in **one PostgreSQL transaction** (Transactional Outbox), so nothing is lost if Kafka is down.
- **At-least-once delivery, handled on purpose:** I tested Kafka being down and a publish that succeeded but failed to mark as published, then built **idempotent consumers** with deduplication, retries, and a **dead-letter queue**.
- **Evidence over guessing:** a RAG + LLM pipeline retrieves runbooks and past incidents so the analysis cites its evidence, with **Redis**-backed incident state.
- **Deployed** with Docker and Kubernetes.

`Go` `PostgreSQL` `Kafka` `Redis` `RAG` `LLMs` `Docker` `Kubernetes`
[Repo →](https://github.com/HariDev-eng/OPSPILOT-REPO-NAME)

<br>

### 🏥 Patient Management Platform — React + 11 Microservices

A healthcare platform built from scratch: a React frontend talking to an API Gateway over 11 backend services, each with its own PostgreSQL database.

| Layer | What's in it |
|---|---|
| 🌐 Edge | API Gateway — routing, JWT authentication, RBAC |
| 🧩 Services | Auth · Patient · Doctor · Nurse · Appointment · Diagnosis · Prescription · Billing · Inventory · Analytics |
| 📨 Messaging | **gRPC** (Protocol Buffers) for synchronous calls, **Kafka** for async domain events |
| 🚢 Delivery | Docker · **Kubernetes** · **Jenkins** CI/CD |

`Java` `Spring Boot` `React` `Kafka` `gRPC` `PostgreSQL` `Docker` `Kubernetes` `Jenkins`
[Backend Repo](https://github.com/HariDev-eng/Patient-Management-System) · [Frontend Repo](https://github.com/HariDev-eng/patient-management-ui)

<br>

### 🎫 Support Ticket & SLA Tracker

A GraphQL backend for support tickets with a **business-hours SLA engine**.

- **Strict ticket lifecycle:** create, assign, comment, change status, and resolve — invalid status transitions are rejected, and first response is detected automatically.
- **SLA engine:** business-hours and timezone-aware deadline calculation, covered by unit tests.
- **Auth and API design:** JWT register/login, cursor pagination, schema-first GraphQL.
- **Foundations:** TypeScript in strict mode, PostgreSQL with Prisma migrations, Docker Compose.

`TypeScript` `GraphQL Yoga` `PostgreSQL` `Prisma` `JWT` `Docker Compose`
[Repo →](https://github.com/HariDev-eng/SLA-TRACKER-REPO-NAME)

<br>

## 🧰 Other Projects

<table>
<tr>
<td width="50%" valign="top">

### 🎬 Concurrent Movie Seat Booking
Preventing double-booking under heavy concurrency — **100,000 concurrent requests**, no double-bookings. Benchmarks three strategies:
- ✅ In-Memory
- ✅ Mutex Protected (`sync.RWMutex`)
- ✅ Redis Atomic `SET NX`

`Go` `Redis` `Goroutines` `Clean Architecture`
[Repo →](https://github.com/HariDev-eng/concurrent-movie-booking)

</td>
<td width="50%" valign="top">

### 🔗 Event-Driven Webhook Processing
A webhook platform inspired by Stripe and GitHub, built to understand asynchronous event delivery.
- Retry mechanism with async workers
- Producer/consumer architecture on RabbitMQ

`Go` `RabbitMQ` `Webhooks`
[Repo →](https://github.com/HariDev-eng/Event-Driven-Webhook-Processing-System)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📝 Blog Platform
A secure REST backend with JWT authentication, Spring Security, and role-based access control.

`Spring Boot` `Spring Security` `JWT` `PostgreSQL`
[Repo →](https://github.com/HariDev-eng/Blog-App)

</td>
<td width="50%" valign="top">

### 📚 Backend Architecture Handbook
Living documentation of the architectural decisions behind these projects — the "why," not just the "what."

`Documentation` `ADRs`

</td>
</tr>
</table>

<br>

## 🛠 Tech Stack

<div align="center">

**Languages**

![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

**Backend**

![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white)
![gRPC](https://img.shields.io/badge/gRPC-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white)
![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=for-the-badge&logo=graphql&logoColor=white)
`REST APIs` `Protocol Buffers` `Spring Security` `JWT` `Webhooks`

**AI**

`RAG` `LLMs` `Embeddings` `Vector Search` `Structured LLM Output`

**Databases**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)

**DevOps & Tools**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Cypress](https://img.shields.io/badge/Cypress-17202C?style=for-the-badge&logo=cypress&logoColor=white)

*Currently learning:*

![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white)

</div>

<br>

## 📊 GitHub Insights

<div align="center">

![Followers](https://img.shields.io/github/followers/HariDev-eng?label=Followers&style=for-the-badge&color=2E9EF7&logo=github&logoColor=white)
![Patient Management Stars](https://img.shields.io/github/stars/HariDev-eng/Patient-Management-System?label=Patient%20Platform%20Stars&style=for-the-badge&color=F7DF1E&logo=github&logoColor=black)
![Last Commit](https://img.shields.io/github/last-commit/HariDev-eng/Patient-Management-System?label=Last%20Commit&style=for-the-badge&color=47A248&logo=github&logoColor=white)

<img src="https://github-readme-streak-stats.herokuapp.com?user=HariDev-eng&theme=tokyonight&hide_border=true" width="600"/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=HariDev-eng&theme=tokyo-night&hide_border=true" width="600"/>

</div>

<br>

## 🌱 Beyond Code

🏋️ Working out · 📚 Reading about distributed systems and software architecture · 📝 Documenting what I learn · 🧩 Solving algorithmic problems · 🚀 Building side projects to test new ideas

<br>

## 🎯 2026 Goals

- [x] Build a distributed healthcare platform
- [x] Deploy it with Docker and Kubernetes
- [x] Build a CI/CD pipeline (Jenkins)
- [x] Build an AI incident-analysis platform (OpsPilot)
- [ ] Learn AWS
- [ ] Complete the Backend Architecture Handbook
- [ ] Contribute to Open Source
- [ ] Land a Backend Engineer role

<br>

<div align="center">

*Building in public — reach out if you're working on distributed systems too.*

</div>
