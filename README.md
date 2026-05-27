<div align="center">

<!-- HEADER WAVE BANNER -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:7c3aed,50:4f46e5,100:0f172a&height=220&section=header&text=Mayur%20Bhusare&fontSize=65&fontColor=ffffff&fontAlignY=40&desc=Backend%20%26%20Distributed%20Systems%20Engineer&descAlignY=60&descSize=20&descColor=c4b5fd&animation=fadeIn&fontAlign=50" />

</div>

<!-- TYPING SVG - FIXED -->
<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&duration=3000&pause=1000&color=A78BFA&center=true&vCenter=true&random=false&width=600&height=60&lines=Building+Fault-Tolerant+Architectures+%F0%9F%94%A5;Queue+Systems+%7C+Workers+%7C+DLQ+%F0%9F%94%81;At-Least-Once+Delivery+Semantics+%F0%9F%9B%A1%EF%B8%8F;Distributed+Systems+in+Go+%F0%9F%90%B9;Reliable+systems+expect+failure+%E2%9A%99%EF%B8%8F)](https://git.io/typing-svg)

</div>

<div align="center">

[![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:mayurbhusare8262@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](YOUR_LINKEDIN_URL)
[![LeetCode](https://img.shields.io/badge/LeetCode_1665-FFA116?style=for-the-badge&logo=leetcode&logoColor=black)](YOUR_LEETCODE_URL)
[![Portfolio](https://img.shields.io/badge/Portfolio-7c3aed?style=for-the-badge&logo=vercel&logoColor=white)](YOUR_PORTFOLIO_URL)

![Profile Views](https://komarev.com/ghpvc/?username=bhusareMayur&color=7c3aed&style=flat-square&label=Profile+Views)

</div>

---

<table>
<tr>
<td width="55%" valign="top">

## 🧑‍💻 About Me

```yaml
name     : Mayur Bhusare
role     : Backend & Distributed Systems Engineer
location : India 🇮🇳
status   : Building GoQueue++ in Go 🚀
focus    : Systems that survive real-world failure
dsaRating: 1665 | 500+ Problems Solved
```

I don't just write backend code — I **engineer reliability**.

My obsession is understanding *why* systems fail  
and building primitives that make them **recover**.

- ⚙️ Deep into **queues, retries, DLQs, idempotency**
- 🐹 Mastering **Go** for high-performance infra
- 📊 Heavy focus on **observability** & failure modes
- 🔬 Always learning beyond coursework

</td>
<td width="45%" valign="top" align="center">

<br/>

<img src="https://raw.githubusercontent.com/platane/snk/output/github-contribution-grid-snake-dark.svg" width="100%" alt="snake"/>

</td>
</tr>
</table>

---

## ⚡ Tech Stack

<div align="center">

<img src="https://skillicons.dev/icons?i=go,nodejs,js,python,java,cpp&perline=6&theme=dark" />
<br/><br/>
<img src="https://skillicons.dev/icons?i=express,redis,rabbitmq,mysql,mongodb,docker&perline=6&theme=dark" />
<br/><br/>
<img src="https://skillicons.dev/icons?i=jest,git,github,linux,vscode&perline=5&theme=dark" />

</div>

---

## 🚀 Featured Projects

<details open>
<summary><b>🔥 Scalable Multi-Channel Notification System</b></summary>
<br/>

> Async notification delivery — Email · SMS · Push — engineered for real-world failure.

<div align="center">

```
  ┌──────────┐    ┌─────────────┐    ┌──────────────────┐    ┌──────────────────┐
  │  Client  │───▶│  REST API   │───▶│    RabbitMQ      │───▶│   Worker Pool    │
  └──────────┘    └─────────────┘    │  Queues/Routing  │    └────────┬─────────┘
                                     └──────────────────┘             │
                                              │               ┌───────▼──────────┐
                                        ┌─────▼──────┐        │  Email / SMS     │
                                        │ Retry Queue│        │  Push Delivery   │
                                        └─────┬──────┘        └──────────────────┘
                                              │
                                        ┌─────▼──────┐
                                        │    DLQ     │
                                        └────────────┘
```

</div>

**Stack:** `Node.js` `RabbitMQ` `Docker` `MySQL` `k6`

| ⚙️ Engineering | 🛡️ Reliability |
|---|---|
| Worker-based async processing | At-least-once delivery semantics |
| Retry Queues + Dead Letter Queue | Worker crash recovery |
| Idempotent consumers (no duplicates) | Fault isolation under burst traffic |
| Horizontal worker scalability | Queue-based service decoupling |
| Structured logging + observability | Retry handling for transient failures |
| k6 load testing | Graceful degradation |

[![View Repo](https://img.shields.io/badge/GitHub-notification--system-0D1117?style=for-the-badge&logo=github)](https://github.com/bhusareMayur/notification-system)

</details>

---

<details open>
<summary><b>⚙️ resilient-queue — Open Source Redis Job Queue</b></summary>
<br/>

> Redis-backed, fault-tolerant job queue focused on the primitives that matter.

<div align="center">

```
  Enqueue ──▶ Redis (LPUSH) ──▶ Worker (BLPOP) ──▶ Execute Handler
                                                          │
                                             ┌────────────┴────────────┐
                                          ✅ Done              ❌ Failure
                                                                    │
                                                         Exponential Backoff
                                                                    │
                                                         ┌──────────┴──────────┐
                                                        No                    Yes
                                                         │                     │
                                                    Retry Queue           💀 Dead Letter Queue
```

</div>

**Stack:** `Node.js` `Redis` `BLPOP` `Jest`

- 🔂 Exponential backoff retries with jitter
- 💀 Dead Letter Queue for exhausted jobs
- 🔑 Idempotency key support
- 🛑 Graceful shutdown (drain before exit)
- ✅ Full Jest test coverage
- 🌍 Open-source contributor friendly

[![View Repo](https://img.shields.io/badge/GitHub-resilient--queue-0D1117?style=for-the-badge&logo=github)](https://github.com/bhusareMayur/resilient-queue)

</details>

---

<details>
<summary><b>🏥 NAMASTE ↔ ICD-11 Healthcare Mapping Platform</b></summary>
<br/>

> Bridging traditional medicine and global health standards through NLP and microservices.

**Stack:** `Node.js` `Python` `NLP (TF-IDF)` `FHIR` `REST APIs`

- 🔍 Semantic search with TF-IDF + cosine similarity
- 🏥 FHIR-compliant healthcare output
- 🧩 Microservice architecture
- 🌐 REST-based inter-service communication

[![View Repo](https://img.shields.io/badge/GitHub-Namaste--ICD11-0D1117?style=for-the-badge&logo=github)](https://github.com/bhusareMayur/Namaste-ICD11)
[![Live Demo](https://img.shields.io/badge/Live_Demo-00C7B7?style=for-the-badge&logo=render&logoColor=white)](https://namaste-icd11.onrender.com)

</details>

---

## 🏗️ Currently Building

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=0:7c3aed,100:4f46e5&height=80&text=GoQueue%2B%2B&fontSize=42&fontColor=ffffff&fontAlign=50&desc=Distributed+Job+Processing+Engine+%E2%80%94+Written+in+Go&descSize=15&descColor=c4b5fd&descAlign=50&animation=twinkling" width="80%"/>

</div>

<br/>

```go
// GoQueue++ — Engineered for production failure scenarios
type Engine struct {
    Language      string   // "Go — concurrency-first"
    Delivery      string   // "at-least-once guaranteed"
    RetryPolicy   Backoff  // exponential with jitter
    DLQ           bool     // true — always
    CrashRecovery bool     // true — workers self-heal
    Observability []string // metrics · traces · structured logs
    WorkerModel   string   // goroutine pools + channels
    FaultTolerant bool     // true — by design, not accident
}
```

<div align="center">

| Feature | Status |
|---|:---:|
| 🔁 At-least-once delivery | 🔨 Building |
| 💀 Retry + Dead Letter Queue | 🔨 Building |
| 🛑 Worker crash recovery | 🔨 Building |
| 📊 Metrics + Structured Logs | 🔨 Building |
| ⚡ Goroutine worker pools | 🔨 Building |
| 🧪 Chaos & fault injection tests | 📋 Planned |

</div>

---

## 📊 GitHub Stats

<div align="center">

<img height="195px" src="https://github-readme-stats.vercel.app/api?username=bhusareMayur&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=a78bfa&icon_color=a78bfa&text_color=c9d1d9&count_private=true" />
<img height="195px" src="https://github-readme-stats.vercel.app/api/top-langs/?username=bhusareMayur&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=a78bfa&text_color=c9d1d9&langs_count=8" />

</div>

<div align="center">

<img src="https://streak-stats.demolab.com/?user=bhusareMayur&theme=tokyonight&hide_border=true&background=0d1117&ring=a78bfa&fire=ff6b6b&currStreakLabel=a78bfa" />

</div>

<div align="center">

<img src="https://github-profile-trophy.vercel.app/?username=bhusareMayur&theme=darkhub&no-frame=true&no-bg=true&margin-w=4&column=7" />

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=rect&color=0:0f172a,100:1e1b4b&height=2" width="100%"/>

<br/>

```
  ╔══════════════════════════════════════════════════════════════════════╗
  ║  "Reliable systems are built by engineers who expect failure."       ║
  ║                                                          — Mayur     ║
  ╚══════════════════════════════════════════════════════════════════════╝
```

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,50:4f46e5,100:7c3aed&height=120&section=footer"/>

</div>
