<div align="center">

<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=26&duration=3000&pause=1200&color=2E9EF7&center=true&vCenter=true&width=650&lines=Hi%2C+I'm+Hari+Pradap+%F0%9F%91%8B;Backend+Engineer;Distributed+Systems+Builder;Go+%7C+Spring+Boot+%7C+Kafka+%7C+RabbitMQ" alt="Typing SVG" />

[![GitHub](https://img.shields.io/badge/GitHub-HariDev--eng-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/HariDev-eng)
![Focus](https://img.shields.io/badge/Focus-Distributed%20Systems-2E9EF7?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Open%20to%20Backend%20Roles-brightgreen?style=for-the-badge)

</div>

<br>

## 🚀 About Me

I'm a backend developer passionate about building scalable systems and understanding **why** software is designed the way it is.

I graduated with a **B.Tech in Information Technology** and completed a **10-month internship at Marmin Technologies**, where I worked on REST APIs, financial document workflows, webhook delivery systems, RabbitMQ, a SaaS compliance platform, PostgreSQL, and Go backend services.

Today I'm focused on learning backend engineering by building **real distributed systems** instead of isolated tutorials. My goal isn't just to write code — it's to understand architecture, scalability, and the engineering trade-offs behind production software.

> *Learn by Building • Improve by Refactoring • Understand by Documenting*

<br>

## 🏥 Flagship Project — Distributed Patient Management Platform

A healthcare platform built from scratch using **microservices** and **event-driven architecture** — my primary vehicle for learning backend engineering properly.

```
                              React Frontend
                                    │
                                    ▼
                              API Gateway
                                    │
        ┌───────────┬──────────────┼──────────────┬────────────┐
        ▼            ▼              ▼              ▼            ▼
   Patient Svc   Doctor Svc     Nurse Svc    Appointment Svc  Auth Svc
        │                                          │
        │                                          ▼
        │                                   Diagnosis Svc
        ▼
   Inventory Svc                          Notification Svc (Go)
        │                                          │
        └──────────────┬───────────────────────────┘
                        ▼
              REST · gRPC · Kafka · RabbitMQ
                        │
                        ▼
                 PostgreSQL · Redis
```

### Services & Status

| Service | Responsibility | Status |
|---|---|:---:|
| 🌐 API Gateway | Centralized routing & request forwarding | ✅ |
| 👤 Patient Service | Registration & profile management | ✅ |
| 👨‍⚕️ Doctor Service | Profiles, availability, specialization | ✅ |
| 🩺 Nurse Service | Nurse assignment & ward management | ✅ |
| 📅 Appointment Service | Scheduling & lifecycle | ✅ |
| 🧾 Diagnosis Service | Medical diagnosis & patient history | ✅ |
| 📦 Inventory Service | Medical inventory management | ✅ |
| 🔔 Notification Service (Go) | Email, SMS, in-app notifications | 🚧 |
| 🔐 Authentication Service | JWT authentication & authorization | 🚧 |
| 🐳 Docker Deployment | Containerizing every service | 🚧 |
| ☸️ Kubernetes | Orchestration | 📅 Planned |

### Communication Patterns

<table>
<tr><td width="25%"><b>REST</b></td><td>Client ↔ Gateway, and general external service access.</td></tr>
<tr><td><b>gRPC</b></td><td>High-performance sync calls between services — e.g. Appointment → Patient Verification, Appointment → Doctor Availability.</td></tr>
<tr><td><b>Kafka</b></td><td>Async domain events — e.g. <code>Appointment Created → Kafka → Notification Service</code>.</td></tr>
<tr><td><b>RabbitMQ</b></td><td>Background worker queues — Notification → RabbitMQ → Email / SMS / In-App workers.</td></tr>
</table>

### Concepts Implemented

`Microservices` `Event-Driven Architecture` `CQRS` `Event-Carried State Transfer` `API Gateway` `JWT Authentication` `Protocol Buffers` `Repository Pattern` `Builder Pattern` `Factory Pattern` `Clean Architecture`

**Stack:** `Spring Boot` `Go` `React` `PostgreSQL` `Kafka` `RabbitMQ` `gRPC` `Protocol Buffers` `Docker` `JWT`

🔗 [Backend Repo](https://github.com/HariDev-eng/Patient-Management-System) · [Frontend Repo](https://github.com/HariDev-eng/patient-management-ui)

<br>

## 🧰 Other Projects

<table>
<tr>
<td width="50%" valign="top">

### 🎬 Concurrent Movie Seat Booking
Preventing double-booking under heavy concurrency. Implements and benchmarks three strategies:
- ✅ In-Memory
- ✅ Mutex Protected (`sync.RWMutex`)
- ✅ Redis Atomic `SET NX`

Interface-driven storage, goroutines, and concurrent load testing.

`Go` `Redis` `Goroutines` `REST APIs` `Clean Architecture`
[Repo →](https://github.com/HariDev-eng/concurrent-movie-booking)

</td>
<td width="50%" valign="top">

### 🔗 Event-Driven Webhook Processing
A webhook platform inspired by Stripe and GitHub, built to understand asynchronous event delivery.
- Event-driven processing
- Retry mechanism with async workers
- Producer/consumer architecture on RabbitMQ

`Go` `RabbitMQ` `REST APIs` `Webhooks`
[Repo →](https://github.com/HariDev-eng/Event-Driven-Webhook-Processing-System)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📝 Blog Platform
A secure REST backend with role-based access control.
- JWT Authentication + Spring Security
- Role-Based Access Control
- Categories, tags, full CRUD APIs

`Spring Boot` `Spring Security` `JWT` `PostgreSQL`
[Repo →](https://github.com/HariDev-eng/Blog-App)

</td>
<td width="50%" valign="top">

### 📚 Backend Architecture Handbook
Living documentation of every major architectural decision made across these projects — the "why," not just the "what."

`Documentation` `ADRs`

</td>
</tr>
</table>

<br>

## 🧠 Learning Roadmap

<details>
<summary><b>Backend</b></summary>
<br>

- [x] REST APIs
- [x] Spring Boot
- [x] Go
- [x] gRPC
- [x] Kafka
- [x] RabbitMQ
- [ ] Authentication & Authorization
- [ ] Docker
- [ ] Kubernetes
- [ ] AWS

</details>

<details>
<summary><b>Software Architecture</b></summary>
<br>

- [x] SOLID Principles
- [x] Clean Architecture
- [ ] Domain-Driven Design
- [ ] CQRS
- [ ] Event-Driven Architecture
- [ ] Event-Carried State Transfer
- [ ] Distributed Messaging
- [ ] Architectural Decision Records (ADRs)

</details>

<details>
<summary><b>Distributed Systems</b></summary>
<br>

- [x] Kafka
- [x] RabbitMQ
- [ ] Retry Strategies
- [ ] Dead Letter Queues
- [ ] Transactional Outbox
- [ ] Idempotency
- [ ] Eventual Consistency
- [ ] Distributed Transactions

</details>

```
Backend Development → Microservices → Event-Driven Systems
      → Distributed Systems → Software Architecture
      → Cloud Native Engineering → Platform Engineering
```

<br>

## 🛠 Tech Stack

<div align="center">

**Languages**
<img src="https://skillicons.dev/icons?i=go,java,javascript,python" />

**Backend**
<img src="https://skillicons.dev/icons?i=spring,nodejs" />
`REST APIs` `gRPC` `Kafka` `RabbitMQ` `Protocol Buffers` `Spring Security` `Webhooks`

**Databases**
<img src="https://skillicons.dev/icons?i=postgres,mongodb,redis,mysql" />

**Frontend**
<img src="https://skillicons.dev/icons?i=react,tailwind" />

**DevOps & Tools**
<img src="https://skillicons.dev/icons?i=docker,git,linux" />
*Currently learning:* `Kubernetes` `AWS` `CI/CD` `GitHub Actions` `Terraform`

</div>

<br>

## 📊 GitHub Insights

<div align="center">

<table>
<tr>
<td><img src="https://github-readme-stats.vercel.app/api?username=HariDev-eng&show_icons=true&theme=tokyonight&hide_border=true&rank_icon=github&count_private=true&card_width=420" /></td>
<td><img src="https://github-readme-stats.vercel.app/api/top-langs/?username=HariDev-eng&layout=compact&theme=tokyonight&hide_border=true&card_width=320" /></td>
</tr>
</table>

<img src="https://github-readme-streak-stats.herokuapp.com?user=HariDev-eng&theme=tokyonight&hide_border=true" width="600"/>

<img src="https://github-profile-trophy.vercel.app/?username=HariDev-eng&theme=tokyonight&no-frame=true&row=1&column=6&margin-w=8" />

<img src="https://github-readme-activity-graph.vercel.app/graph?username=HariDev-eng&theme=tokyo-night&hide_border=true" width="600"/>

</div>

<details>
<summary><b>Cards showing broken?</b> — click for the fix</summary>
<br>

The shared `github-readme-stats.vercel.app` instance hits its free-tier GitHub API rate limit constantly — this happens to a lot of profiles, not just yours. Fixes, in order of effort:

1. **Wait it out** — the shared instance often recovers within 10–30 minutes.
2. **Cache-bust** — append `&cache_seconds=1800` to each URL to force a fresh render.
3. **Self-host (permanent fix)** — fork [anuraghazra/github-readme-stats](https://github.com/anuraghazra/github-readme-stats), deploy to your own free Vercel project, generate a GitHub PAT (classic, no expiry, `repo` + `read:user` scopes), set it as `PAT_1` in your Vercel env vars, then swap the domain in every URL above for your own deployment. ~10 minutes, and you stop sharing quota with the entire internet.

</details>

<br>

## 🌱 Beyond Code

🏋️ Working out · 📚 Reading about distributed systems and software architecture · 📝 Documenting what I learn · 🧩 Solving algorithmic problems · 🚀 Building side projects to test new ideas

<br>

## 🎯 2026 Goals

- [x] Build a distributed healthcare platform
- [ ] Deploy every service with Docker
- [ ] Learn Kubernetes
- [ ] Learn AWS
- [ ] Build CI/CD pipelines
- [ ] Complete the Backend Architecture Handbook
- [ ] Contribute to Open Source
- [ ] Land a Backend Engineer role

<br>

<div align="center">

*Building in public — reach out if you're working on distributed systems too.*

</div>
