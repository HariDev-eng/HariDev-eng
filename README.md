<div align="center">

<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=26&duration=3000&pause=1200&color=2E9EF7&center=true&vCenter=true&width=760&lines=Hi%2C+I'm+Hari+Pradap+%F0%9F%91%8B;Backend+Engineer;Go+%7C+Java+%7C+Distributed+Systems;Exploring+Applied+AI+%26+RAG" alt="Typing SVG" />

[![GitHub](https://img.shields.io/badge/GitHub-HariDev--eng-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/HariDev-eng)
![Focus](https://img.shields.io/badge/Focus-Backend%20%2B%20Applied%20AI-2E9EF7?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Open%20to%20Backend%20Opportunities-brightgreen?style=for-the-badge)

</div>

---

## 👋 About Me

I'm a backend-focused software engineer interested in building reliable APIs, event-driven systems, and distributed applications. I enjoy understanding the engineering trade-offs behind a system—not just getting it to work.

I hold a **B.Tech in Information Technology** and completed a **10-month internship at Marmin Technologies**. During the internship, I worked on backend microservices, REST APIs, webhooks, RabbitMQ-based asynchronous processing, database design, and Cypress automation for a live SaaS platform.

My current hands-on focus is **Go, Java/Spring Boot, PostgreSQL, messaging systems, and Applied AI**. I learn by building projects, testing failure cases, and documenting the decisions behind the implementation.

> Learn by building · Improve by refactoring · Understand by documenting

## ⭐ Featured Projects

### 🧭 [OpsPilot — AI Incident Intelligence & Response](https://github.com/HariDev-eng/OpsPilot)

An event-driven incident-intelligence prototype that ingests operational events, detects repeated failures, groups them into incidents, and uses RAG with an LLM to generate evidence-referenced investigation summaries and response recommendations.

**What I built**
- Event ingestion through a Go HTTP API, with events and outbox records persisted in a single PostgreSQL transaction.
- Asynchronous event publishing through a transactional outbox and Kafka.
- Idempotent event consumption and Redis-backed sliding-window failure detection.
- Incident context construction, embedding-based retrieval with pgvector, and LLM-generated analysis.
- Evidence validation and an operator workflow for reviewing and approving recommended actions.

**Architecture at a glance**

```text
Events → Go API → PostgreSQL (events + outbox) → Kafka
                                                   ↓
                                      Idempotent consumer
                                                   ↓
                                  Redis detection → Incidents
                                                   ↓
                             RAG (pgvector) + LLM analysis
                                                   ↓
                               Evidence checks → Operator UI
```

**Tech:** Go · PostgreSQL · Kafka · Redis · pgvector · Cloudflare Workers AI · React · TypeScript

- [Live application](https://opspilot-7q8.pages.dev)
- [Backend API](https://opspilot-7o2e.onrender.com)
- [Architecture documentation](https://github.com/HariDev-eng/OpsPilot/tree/main/docs/architecture)

**Status:** V1 portfolio prototype deployed and exercised with synthetic events. It is not represented as production-ready; authentication/authorization, broader automated coverage, and operational hardening remain follow-up work.

### 🏥 [Patient Management Platform](https://github.com/HariDev-eng/Patient-Management-System)

A healthcare application structured around an API Gateway and backend services for core clinical and administrative workflows.

- Backend services cover authentication, patients, doctors, nurses, appointments, diagnosis, prescriptions, billing, inventory, and analytics.
- Uses gRPC/Protocol Buffers for service-to-service communication and Kafka for asynchronous domain events.
- Built with Spring Boot and PostgreSQL, with Docker, Kubernetes, and Jenkins in the delivery workflow.

**Tech:** Java · Spring Boot · PostgreSQL · gRPC · Kafka · Docker · Kubernetes · Jenkins

- [Backend repository](https://github.com/HariDev-eng/Patient-Management-System)
- [Frontend repository](https://github.com/HariDev-eng/Patient-Management-System-UI)

## 🧰 Other Projects

### 🎫 [Ticket Booking System](https://github.com/HariDev-eng/Ticket-Booking-Sytem)

A backend project exploring ticket-booking workflows and concurrency-safe reservation design.

**Tech:** Go · Redis · PostgreSQL

### 🔗 [Event-Driven Webhook Processing System](https://github.com/HariDev-eng/Event-Driven-Webhook-Processing-System)

A webhook-processing project exploring asynchronous event delivery through producer/consumer components, RabbitMQ, and retry handling.

**Tech:** Go · RabbitMQ · Webhooks

## 🛠️ Tech Stack

**Languages**

![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

**Backend & APIs**

![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=for-the-badge&logo=graphql&logoColor=white)
![gRPC](https://img.shields.io/badge/gRPC-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white)
![Kafka](https://img.shields.io/badge/Apache%20Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white)

`REST APIs` `Webhooks` `JWT` `Spring Security` `Protocol Buffers`

**Applied AI**

`LLMs` `RAG` `Embeddings` `Vector Search` `Structured Output`

**Databases**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)

**Frontend & DevOps**

![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white)
![Cypress](https://img.shields.io/badge/Cypress-17202C?style=for-the-badge&logo=cypress&logoColor=white)

## 📊 GitHub Activity

<div align="center">

![GitHub followers](https://img.shields.io/github/followers/HariDev-eng?label=Followers&style=for-the-badge&color=2E9EF7&logo=github&logoColor=white)
![OpsPilot stars](https://img.shields.io/github/stars/HariDev-eng/OpsPilot?label=OpsPilot%20Stars&style=for-the-badge&color=F7DF1E&logo=github&logoColor=black)

<img src="https://github-readme-streak-stats.herokuapp.com?user=HariDev-eng&theme=tokyonight&hide_border=true" width="600" alt="GitHub contribution streak" />

<img src="https://github-readme-activity-graph.vercel.app/graph?username=HariDev-eng&theme=tokyo-night&hide_border=true" width="600" alt="GitHub activity graph" />

</div>

## 🌱 Current Focus

- Deepening backend engineering fundamentals: concurrency, databases, API design, and distributed systems.
- Building practical Applied AI systems with LLMs, RAG, embeddings, and evaluation.
- Improving problem-solving skills through consistent DSA and SQL practice.
- Looking for backend engineering opportunities where I can build and learn from real systems.

## 🤝 Connect

- GitHub: [HariDev-eng](https://github.com/HariDev-eng)

<div align="center">

*Building in public. Always curious about systems, reliability, and thoughtful engineering.*

</div>
