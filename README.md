<div align="center">

<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=500&size=24&duration=3000&pause=1200&color=2E9EF7&center=true&vCenter=true&width=600&lines=Hi%2C+I'm+Hari+Pradap;Backend+Engineer;Distributed+Systems+Enthusiast" alt="Typing SVG" />

**Backend Engineer · Microservices & Distributed Systems**

[![GitHub](https://img.shields.io/badge/GitHub-HariDev--eng-181717?style=flat-square&logo=github)](https://github.com/HariDev-eng)
[![Location](https://img.shields.io/badge/Focus-Backend%20Engineering-2E9EF7?style=flat-square)](#)

</div>

<br>

## About

I'm a backend developer who learns by building real systems instead of tutorials. B.Tech in Information Technology, followed by a 10-month internship at Marmin Technologies building REST APIs, financial document workflows, webhook delivery pipelines, and a SaaS compliance platform on Go + PostgreSQL + RabbitMQ.

Right now I'm going deep on **distributed systems** — designing services, wiring them together with events, and documenting every architectural decision along the way as I build toward a backend engineering role in 2026.

> *Learn by building. Improve by refactoring. Understand by documenting.*

<br>

## 🏥 Flagship Project — Distributed Patient Management Platform

A healthcare platform built from scratch on microservices and event-driven architecture — my main vehicle for learning distributed systems properly.

<div align="center">
<img width="600" alt="architecture diagram" src="./architecture.svg"/>
</div>

**Services**

| Service | Role | Status |
|---|---|:---:|
| API Gateway | Centralized routing | ✅ |
| Patient / Doctor / Nurse | Core domain services | ✅ |
| Appointment | Scheduling & lifecycle | ✅ |
| Diagnosis | Records & history | ✅ |
| Inventory | Medical stock management | ✅ |
| Notification (Go) | Email / SMS / in-app | 🚧 |
| Authentication | JWT auth & authorization | 🚧 |

**Communication layer:** REST (client-facing) · gRPC (service-to-service, e.g. Appointment → Patient/Doctor) · Kafka (async domain events) · RabbitMQ (background workers: email/SMS/in-app)

**Concepts applied:** CQRS · Event-Carried State Transfer · API Gateway · Repository/Builder/Factory patterns · Clean Architecture

**Stack:** `Spring Boot` `Go` `React` `PostgreSQL` `Kafka` `RabbitMQ` `gRPC` `Docker` `JWT`

🔗 [Backend](https://github.com/HariDev-eng/Patient-Management-System) · [Frontend](https://github.com/HariDev-eng/patient-management-ui)

**Next up:** Docker deployment → Kubernetes → AWS → CI/CD → distributed tracing

<br>

## Other Projects

<table>
<tr>
<td width="50%" valign="top">

**🎬 Concurrent Movie Seat Booking**
Preventing double-booking under load — three synchronization strategies compared: in-memory, mutex-protected, and Redis atomic `SET NX`, with concurrent load-test benchmarks.

`Go` `Redis` `Goroutines`
[Repo →](https://github.com/HariDev-eng/concurrent-movie-booking)

</td>
<td width="50%" valign="top">

**🔗 Event-Driven Webhook Processing**
A Stripe/GitHub-inspired webhook delivery system with retries and async producer/consumer workers built on RabbitMQ.

`Go` `RabbitMQ` `Webhooks`
[Repo →](https://github.com/HariDev-eng/Event-Driven-Webhook-Processing-System)

</td>
</tr>
<tr>
<td width="50%" valign="top">

**📝 Blog Platform**
Secure REST backend with JWT auth, Spring Security, and role-based access control.

`Spring Boot` `Spring Security` `JWT` `PostgreSQL`
[Repo →](https://github.com/HariDev-eng/Blog-App)

</td>
<td width="50%" valign="top">

**📚 Backend Architecture Handbook**
Living notes and ADRs documenting the trade-offs behind every design decision in the projects above.

`Documentation` `ADRs`

</td>
</tr>
</table>

<br>

## Tech Stack

<div align="center">

**Languages & Frameworks**
<img src="https://skillicons.dev/icons?i=go,java,spring,javascript,python,react" />

**Data & Messaging**
<img src="https://skillicons.dev/icons?i=postgres,mongodb,redis,mysql,kafka,rabbitmq" />

**Infra & Tools**
<img src="https://skillicons.dev/icons?i=docker,kubernetes,aws,git,linux" />

</div>

*Currently learning: Kubernetes · AWS · CI/CD · Terraform · Domain-Driven Design*

<br>

## GitHub Stats

<div align="center">

<table>
<tr>
<td><img src="https://github-readme-stats.vercel.app/api?username=HariDev-eng&show_icons=true&theme=tokyonight&hide_border=true&rank_icon=github&count_private=true&card_width=420" /></td>
<td><img src="https://github-readme-stats.vercel.app/api/top-langs/?username=HariDev-eng&layout=compact&theme=tokyonight&hide_border=true&card_width=320" /></td>
</tr>
</table>

<img src="https://github-readme-streak-stats.herokuapp.com?user=HariDev-eng&theme=tokyonight&hide_border=true" width="600"/>

<img src="https://github-profile-trophy.vercel.app/?username=HariDev-eng&theme=tokyonight&no-frame=true&row=1&column=6&margin-w=8" />

</div>

**If these render as broken images:** it's the shared `github-readme-stats.vercel.app` instance hitting its free-tier GitHub API rate limit — this happens to a lot of profiles, not just yours, and comes and goes. Three ways to actually fix it, in order of effort:

1. **Do nothing** — wait 10–30 min and refresh; the shared instance often recovers on its own.
2. **Cache-bust** — append `&cache_seconds=1800` to each URL to force a fresh render instead of a stale cached broken image.
3. **Self-host (permanent fix)** — fork [anuraghazra/github-readme-stats](https://github.com/anuraghazra/github-readme-stats), deploy it to your own free Vercel project, generate a GitHub Personal Access Token (classic, no expiry, `repo` + `read:user` scopes), add it as a `PAT_1` env var on your Vercel deployment, then swap `github-readme-stats.vercel.app` in every URL above for your own `your-project.vercel.app`. Takes about 10 minutes and you're no longer sharing quota with the entire internet — same fix applies to the streak-stats and trophy widgets if you self-host those forks too.

<br>

## 2026 Goals

- [x] Design & build a distributed healthcare platform
- [ ] Ship every service with Docker + Kubernetes
- [ ] Learn AWS and build CI/CD pipelines
- [ ] Finish the Backend Architecture Handbook
- [ ] Contribute to open source
- [ ] Land a backend engineer role

<br>

<div align="center">

*Building in public. Reach out if you're working on distributed systems too.*

</div>
