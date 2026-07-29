<div align="center">

![header](https://capsule-render.vercel.app/api?type=waving&height=220&text=Mayur%20Bhusare&fontAlign=50&fontAlignY=38&color=gradient&customColorList=12,20,24&desc=Backend%20Distributed%20Systems%20Engineer&descAlignY=58&descSize=20&animation=fadeIn)

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&pause=1000&color=A78BFA&center=true&vCenter=true&width=650&lines=Backend+Distributed+Systems;Queue+Workers+DLQ;Reliable+Systems+Expect+Failure;GoQueue+Live)](https://git.io/typing-svg)

<br/>

[![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:mayurbhusare8262@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mayur-bhusare/)
[![Portfolio](https://img.shields.io/badge/Portfolio-7c3aed?style=for-the-badge&logo=vercel&logoColor=white)](https://bhusaremayur.github.io/portfolio/)

![Profile Views](https://komarev.com/ghpvc/?username=bhusareMayur&color=7c3aed&style=flat-square&label=Profile+Views)

</div>

---

## 🧑‍💻 About Me

```yaml
name     : Mayur Bhusare
role     : Backend & Distributed Systems Engineer
location : Pune, India
status   : GoQueue live - 2.9k req/sec, zero job loss
focus    : Systems that survive real-world failure
DSA      : LeetCode Knight | Contest Rating 1960+ | Top 3.05% Globally
```

I don't just write backend code - I **engineer reliability**.

My obsession is understanding *why* systems fail
and building primitives that make them **recover**.

- Deep into queues, retries, DLQs, idempotency
- Building production infra in Go
- Heavy focus on observability and failure modes
- Always learning beyond coursework

---

## ⚡ Tech Stack

**Languages:** Go (Golang), JavaScript, Java, Python

**Backend & APIs:** Go, Node.js, Express.js, REST APIs, Microservices-oriented design

**Distributed Systems:** Redis, RabbitMQ, Concurrent Worker Pools, Retry Orchestration, DLQ, Visibility Timeout, Async Processing

**Observability:** Prometheus, Grafana, Structured Logging

**Reliability:** Fault Tolerance, Idempotency, Rate Limiting, Graceful Shutdown, Backpressure, Load Shedding

**Databases:** PostgreSQL, MongoDB, MySQL

**Cloud & Infra:** Docker, AWS (EC2, S3, RDS, Lambda), Linux

**Testing & Tools:** k6 (Load Testing), Git, Postman

**Fundamentals:** System Design, OS, DBMS, Computer Networks, OOP

---

## 🚀 Featured Projects

### GoQueue - Distributed Background Job Processing Engine
`Go` `Redis` `PostgreSQL` `Docker` `Prometheus` `Grafana` `k6`

Architected a distributed background job engine in Go (inspired by Sidekiq/BullMQ) using Redis for high-throughput queueing and PostgreSQL for durable job state; supports fan-out, priority queues, and deferred scheduling. Built concurrent worker pools with goroutines: exponential backoff retry, DLQ routing, visibility timeouts, graceful shutdown, stuck-job recovery via background reaper, and backpressure via queue-depth monitoring. Instrumented Prometheus/Grafana dashboards (queue depth, throughput, retry rates, worker utilization, p50/p95/p99 latency); k6 load-tested to 10k concurrent submissions at ~2.9k req/sec with zero crashes or job loss.

[GitHub](https://github.com/bhusareMayur/GoQueue)

### Scalable Multi-Channel Notification System
`Node.js` `RabbitMQ` `Docker` `MySQL` `k6`

Designed an asynchronous notification pipeline for Email/SMS/Push channels using RabbitMQ fanout exchanges with per-channel retry handling, DLQ isolation, and idempotent consumers. Sustained p99 delivery latency under 450ms under load testing with zero message loss across all retry and failure scenarios.

[GitHub](https://github.com/bhusareMayur/notification-system)

### JobPulse - Real-Time Job Market Demand Platform
`Node.js` `Express` `PostgreSQL` `Redis`

Decoupled background worker ingesting 100+ job listings daily across 40+ CS roles without blocking the request path. Redis caching cut DB query latency from ~500ms to ~8ms (98% reduction). Enforced per-IP rate limiting at 60 req/min to prevent abuse under high-concurrency campus-scale traffic.

[GitHub](https://github.com/bhusareMayur/JobPulse)

### resilient-queue - Open Source Redis Job Queue
`Node.js` `Redis` `BLPOP` `Semantic Versioning`

Published a Redis-backed queue library with retry orchestration, DLQ routing, idempotency guards, and graceful shutdown, available on npm with 500+ downloads. Managed semantic versioning and community contributions.

[GitHub](https://github.com/bhusareMayur/resilient-queue) · [npm]([https://www.npmjs.com/package/resilient-queue](https://www.npmjs.com/package/@mayurbhusare/resilient-queue)

---

## 💼 Experience

**Backend Developer - Lagnify (Freelance)** · Jun 2025 - Nov 2025

- Designed and built a 3-module REST API backend (auth, orders, admin) for lagnify.com using Node.js and MongoDB
- Owned the full deployment lifecycle on Render: DNS configuration, HTTPS provisioning, environment management, and production monitoring for reliable backend availability

---

## 🎓 Education

**B.Tech - Computer Engineering**, JSPM RSCOE, Pune - 2023 - 2027 - CGPA: 8.95

---

## 🧠 Engineering Principles

- Reliability: expect failure, design for recovery, idempotency first
- Observability: log everything (structured), trace distributed systems, alert on anomaly
- Architecture: decouple with queues, retry transient failures, isolate fault zones
- Philosophy: if it's not tested, it's not working; build for recovery, not perfection; failure is expected

---

## 🏆 Achievements

- LeetCode Knight | Contest Rating 1960+ | Top 3.05% Globally
- Weekly Contest 508 - Rank 361/37,970 (Top 0.95%)
- Recursion 3.0 - Runner-up

---

<div align="center">

<br/>

*- Mayur Bhusare*

> **"Reliable systems are built by engineers who expect failure."**

<br/>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,50:4f46e5,100:7c3aed&height=130&section=footer"/>

</div>
