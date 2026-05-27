<div align="center">

```
██████╗  █████╗  ██████╗██╗  ██╗███████╗███╗   ██╗██████╗
██╔══██╗██╔══██╗██╔════╝██║ ██╔╝██╔════╝████╗  ██║██╔══██╗
██████╔╝███████║██║     █████╔╝ █████╗  ██╔██╗ ██║██║  ██║
██╔══██╗██╔══██║██║     ██╔═██╗ ██╔══╝  ██║╚██╗██║██║  ██║
██████╔╝██║  ██║╚██████╗██║  ██╗███████╗██║ ╚████║██████╔╝
╚═════╝ ╚═╝  ╚═╝ ╚═════╝╚═╝  ╚═╝╚══════╝╚═╝  ╚═══╝╚═════╝
```

### `> Building systems that survive the real world.`

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=18&duration=3000&pause=800&color=00D9FF&center=true&vCenter=true&width=600&lines=Backend+%26+Distributed+Systems+Engineer;Fault-Tolerant+Architecture+Designer;Queue+Systems+%7C+Worker+Pools+%7C+Observability;Go+%7C+Node.js+%7C+Redis+%7C+RabbitMQ;%22Reliable+systems+expect+failure.%22)](https://git.io/typing-svg)

</div>

---

<img align="right" width="360" src="https://raw.githubusercontent.com/platane/snk/output/github-contribution-grid-snake-dark.svg" alt="snake animation"/>

## `$ whoami`

```yaml
name:     Mayur Bhusare
role:     Backend & Distributed Systems Engineer
focus:    Reliability · Scalability · Fault Tolerance
status:   Building GoQueue++ in Go 🚀
location: India 🇮🇳
email:    mayurbhusare8262@gmail.com
```

**I build systems that don't just work — they survive.**

- ⚙️ Obsessed with **asynchronous architectures** and **failure recovery**
- 🔁 Deep experience with **queues, retries, DLQs, and idempotency**
- 📡 Strong focus on **observability** and understanding *why* systems fail
- 🐹 Currently mastering **Go** for concurrent, high-performance systems
- 🧠 500+ DSA problems | LeetCode Rating **1665**

<br clear="right"/>

---

## `$ cat /proc/tech-stack`

<div align="center">

| Layer | Technologies |
|---|---|
| **Languages** | ![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white) |
| **Backend** | ![Express](https://img.shields.io/badge/Express.js-000000?style=flat-square&logo=express&logoColor=white) ![REST](https://img.shields.io/badge/REST_APIs-FF6B35?style=flat-square) |
| **Messaging** | ![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white) |
| **Databases** | ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white) |
| **Infra & DevOps** | ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![k6](https://img.shields.io/badge/k6-7D64FF?style=flat-square&logo=k6&logoColor=white) |
| **Testing** | ![Jest](https://img.shields.io/badge/Jest-C21325?style=flat-square&logo=jest&logoColor=white) |

</div>

---

## `$ ls ~/projects`

<details open>
<summary><b>🔥 Scalable Multi-Channel Notification System</b></summary>

<br/>

> *Async notification delivery at scale — Email, SMS, Push — built to survive failure.*

```
┌─────────────────────────────────────────────────────────────────────┐
│                    SYSTEM ARCHITECTURE                              │
│                                                                     │
│  API Layer  ──►  RabbitMQ  ──►  Worker Pool  ──►  Email/SMS/Push   │
│                     │               │                               │
│                  Retry Queue    DLQ Handler                         │
│                     │               │                               │
│               Exponential       Structured                          │
│                 Backoff           Logging                           │
└─────────────────────────────────────────────────────────────────────┘
```

**Tech:** `Node.js` `RabbitMQ` `Docker` `MySQL` `k6`

| Feature | Detail |
|---|---|
| 🔁 Retry Strategy | Dead Letter Queue + exponential backoff |
| 🛡️ Delivery Guarantee | At-least-once semantics |
| 🔒 Idempotency | Prevents duplicate delivery |
| 📊 Observability | Structured logging for retries & failures |
| ⚡ Scalability | Horizontal worker scaling |
| 🧪 Load Testing | k6 under burst traffic scenarios |

**Reliability concepts implemented:** Worker crash recovery · Queue-based decoupling · Fault isolation under burst traffic

[![Repo](https://img.shields.io/badge/GitHub-notification--system-181717?style=for-the-badge&logo=github)](https://github.com/bhusareMayur/notification-system)

</details>

---

<details open>
<summary><b>⚙️ resilient-queue — Open Source Redis Job Queue</b></summary>

<br/>

> *A Redis-backed, fault-tolerant job queue focused on the primitives that matter.*

```
Job Enqueue ──► BLPOP Worker ──► Execute ──► ✅ Success
                     │                  │
                     │              ❌ Failure
                     │                  │
                     │         Exponential Backoff
                     │                  │
                     │           Max Retries?
                     │            /         \
                     │          No           Yes
                     │           │             │
                     │       Retry Queue    Dead Letter Queue
```

**Tech:** `Node.js` `Redis` `BLPOP` `Jest`

- 🔂 Exponential backoff retries
- 💀 DLQ for exhausted jobs
- 🔑 Idempotency key support
- 🛑 Graceful shutdown handling
- ✅ Full Jest test coverage

[![Repo](https://img.shields.io/badge/GitHub-resilient--queue-181717?style=for-the-badge&logo=github)](https://github.com/bhusareMayur/resilient-queue)

</details>

---

<details>
<summary><b>🏥 NAMASTE ↔ ICD-11 Healthcare Mapping Platform</b></summary>

<br/>

> *Bridging traditional medicine and global health standards through NLP.*

**Tech:** `Node.js` `Python` `NLP` `REST APIs` `FHIR`

- 🔍 TF-IDF + cosine similarity semantic search engine
- 🏥 FHIR-compliant healthcare data outputs
- 🧩 Microservice-based architecture
- 🌐 REST-based inter-service communication

[![Repo](https://img.shields.io/badge/GitHub-Namaste--ICD11-181717?style=for-the-badge&logo=github)](https://github.com/bhusareMayur/Namaste-ICD11)
[![Demo](https://img.shields.io/badge/Live_Demo-namaste--icd11-00C7B7?style=for-the-badge&logo=render)](https://namaste-icd11.onrender.com)

</details>

---

## `$ top -pid current_build`

```
PID: GoQueue++          STATUS: 🔨 BUILDING          CPU: 100%
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

**GoQueue++** — A distributed job processing engine in Go

```go
type GoQueueEngine struct {
    Delivery      string   // "at-least-once"
    RetryPolicy   Backoff  // exponential with jitter
    DLQ           bool     // true
    Observability []string // {"metrics", "traces", "logs"}
    Concurrency   string   // "worker pools + goroutines"
    FaultTolerance bool    // true — always
}
```

> Engineered from the ground up for crash recovery, concurrent processing, and observable failure modes.

---

## `$ cat /etc/engineering.principles`

```
[reliability]
expect_failure         = true
design_for_recovery    = true
idempotency_first      = true

[architecture]
decouple_with_queues   = true
retry_transient_errors = true
isolate_fault_domains  = true

[observability]
log_everything         = structured
trace_distributed_ops  = true
alert_on_anomalies     = true

[philosophy]
"Reliable systems are built by engineers who expect failure."
```

---

## `$ ./stats --github`

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=bhusareMayur&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=00D9FF&icon_color=00D9FF&text_color=ffffff&rank_icon=github)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=bhusareMayur&layout=compact&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=00D9FF&text_color=ffffff)

![GitHub Streak](https://streak-stats.demolab.com?user=bhusareMayur&theme=tokyonight&hide_border=true&background=0D1117&ring=00D9FF&fire=FF6B35&currStreakLabel=00D9FF)

</div>

---

## `$ ping --connect`

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](YOUR_LINKEDIN_URL)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-FF6B35?style=for-the-badge&logo=firefox&logoColor=white)](YOUR_PORTFOLIO_URL)
[![LeetCode](https://img.shields.io/badge/LeetCode-1665_Rating-FFA116?style=for-the-badge&logo=leetcode&logoColor=black)](YOUR_LEETCODE_URL)
[![Email](https://img.shields.io/badge/Email-mayurbhusare8262@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:mayurbhusare8262@gmail.com)

</div>

---

<div align="center">

```
┌──────────────────────────────────────────────────────────────┐
│  "Reliable systems are built by engineers who expect failure."│
│                                          — Mayur Bhusare      │
└──────────────────────────────────────────────────────────────┘
```

![Profile Views](https://komarev.com/ghpvc/?username=bhusareMayur&color=00D9FF&style=flat-square&label=PROFILE+VIEWS)

</div>
