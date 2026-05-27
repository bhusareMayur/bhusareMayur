<div align="center">

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&height=220&text=Mayur%20Bhusare&fontAlign=50&fontAlignY=38&color=gradient&customColorList=12,20,24&desc=Backend%20%26%20Distributed%20Systems%20Engineer&descAlignY=58&descSize=20&animation=fadeIn" width="100%" />
</p>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&duration=3000&pause=1000&color=A78BFA&center=true&vCenter=true&width=650&height=55&lines=Building+Fault-Tolerant+Architectures+%F0%9F%94%A5;Queue+Systems+%7C+Workers+%7C+DLQ+%F0%9F%94%81;At-Least-Once+Delivery+Semantics+%F0%9F%9B%A1%EF%B8%8F;Distributed+Systems+in+Go+%F0%9F%90%B9;Reliable+systems+expect+failure+%E2%9A%99%EF%B8%8F)](https://git.io/typing-svg)

<br/>

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
dsa      : 1665 Rating | 500+ Problems Solved
```

I don't just write backend code — I **engineer reliability**.

My obsession is understanding *why* systems fail  
and building primitives that make them **recover**.

- ⚙️ Deep into **queues, retries, DLQs, idempotency**
- 🐹 Mastering **Go** for high-performance infra
- 📊 Heavy focus on **observability** and failure modes
- 🔬 Always learning beyond coursework

</td>
<td width="45%" valign="top" align="center">

<br/><br/>

<img src="https://raw.githubusercontent.com/platane/snk/output/github-contribution-grid-snake-dark.svg" width="100%" alt="contribution snake"/>

<br/>

```
⚙️  Async Systems       ████████████  100%
🔁  Queue & Retry       ████████████  100%
🛡️  Reliability Eng.   ███████████░   90%
🐹  Go (Learning)       ████████░░░░   65%
📊  Observability       █████████░░░   75%
```

</td>
</tr>
</table>

---

## ⚡ Tech Stack

<div align="center">

**Languages**
<br/>
<img src="https://skillicons.dev/icons?i=go,nodejs,js,python,java,cpp&perline=6&theme=dark" />

<br/><br/>

**Backend · Messaging · Databases**
<br/>
<img src="https://skillicons.dev/icons?i=express,redis,rabbitmq,mysql,mongodb,docker&perline=6&theme=dark" />

<br/><br/>

**Tools & Testing**
<br/>
<img src="https://skillicons.dev/icons?i=jest,git,github,linux,vscode&perline=5&theme=dark" />

</div>

---

## 🚀 Featured Projects

<details open>
<summary><b>🔥 &nbsp;Scalable Multi-Channel Notification System</b> &nbsp;&nbsp;<img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white"/> <img src="https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white"/> <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/> <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white"/></summary>

<br/>

> **Async notification delivery at scale — Email · SMS · Push — engineered to survive burst traffic and worker crashes.**

```
  ┌──────────┐    ┌─────────────┐    ┌──────────────────┐
  │  Client  │───▶│  REST API   │───▶│    RabbitMQ      │
  └──────────┘    └─────────────┘    │  Exchange/Queue  │
                                     └────────┬─────────┘
                                              │
                               ┌──────────────▼──────────────┐
                               │         Worker Pool          │
                               │   (Horizontal Scalability)   │
                               └──────────────┬──────────────┘
                                              │
                          ┌───────────────────┼───────────────────┐
                          ▼                   ▼                   ▼
                       📧 Email            📱 SMS            🔔 Push
                          │                   │                   │
                          └───────────────────┼───────────────────┘
                                              │
                                    ┌─────────▼─────────┐
                                    │    Retry Queue     │
                                    │  (Exp. Backoff)    │
                                    └─────────┬─────────┘
                                              │
                                    ┌─────────▼─────────┐
                                    │   Dead Letter Q    │
                                    │   + Structured     │
                                    │     Logging        │
                                    └───────────────────-┘
```

<table>
<tr>
<td>

**⚙️ Engineering Features**
- ✅ Worker-based async processing
- ✅ Retry queues + Dead Letter Queue
- ✅ Idempotent consumers (zero duplicates)
- ✅ Horizontal worker scalability
- ✅ Structured logging for observability
- ✅ Load tested with k6

</td>
<td>

**🛡️ Reliability Concepts**
- At-least-once delivery semantics
- Worker crash recovery
- Queue-based service decoupling
- Exponential backoff for transient failures
- Fault isolation under burst traffic
- Graceful degradation under load

</td>
</tr>
</table>

[![View Repo](https://img.shields.io/badge/GitHub-notification--system-0D1117?style=for-the-badge&logo=github&logoColor=white)](https://github.com/bhusareMayur/notification-system)

</details>

<br/>

<details open>
<summary><b>⚙️ &nbsp;resilient-queue — Open Source Redis Job Queue</b> &nbsp;&nbsp;<img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white"/> <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white"/> <img src="https://img.shields.io/badge/Jest-C21325?style=flat-square&logo=jest&logoColor=white"/> <img src="https://img.shields.io/badge/Open_Source-ff6b6b?style=flat-square&logo=opensourceinitiative&logoColor=white"/></summary>

<br/>

> **Redis-backed, fault-tolerant job queue with battle-hardened retry primitives.**

```
  ┌─────────────────────────────────────────────────────────────┐
  │                                                             │
  │   Enqueue ──▶ Redis LPUSH ──▶ Worker BLPOP ──▶ Execute     │
  │                                                    │        │
  │                                        ┌──────────┴──────┐ │
  │                                        │                 │ │
  │                                     ✅ Done         ❌ Fail │
  │                                                        │   │
  │                                            Exponential     │
  │                                               Backoff      │
  │                                                  │         │
  │                                       ┌──────────┴──────┐  │
  │                                      No                Yes  │
  │                                       │                 │  │
  │                                  Retry Queue       💀 DLQ  │
  │                                                            │
  └────────────────────────────────────────────────────────────┘
```

- 🔂 Exponential backoff with jitter
- 💀 Dead Letter Queue for exhausted jobs
- 🔑 Idempotency key support
- 🛑 Graceful shutdown — drains before exit
- ✅ Full Jest test coverage
- 🌍 Open-source contributor friendly

[![View Repo](https://img.shields.io/badge/GitHub-resilient--queue-0D1117?style=for-the-badge&logo=github&logoColor=white)](https://github.com/bhusareMayur/resilient-queue)

</details>

<br/>

<details>
<summary><b>🏥 &nbsp;NAMASTE ↔ ICD-11 Healthcare Mapping Platform</b> &nbsp;&nbsp;<img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white"/> <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/> <img src="https://img.shields.io/badge/NLP-TF--IDF-7c3aed?style=flat-square"/> <img src="https://img.shields.io/badge/FHIR-Compliant-00897B?style=flat-square"/></summary>

<br/>

> **Bridging traditional medicine and global health standards through NLP and microservices.**

```
  Traditional Medicine Term
            │
            ▼
  ┌─────────────────────┐
  │   NLP Preprocessing │
  │   (Tokenize/Clean)  │
  └──────────┬──────────┘
             │
             ▼
  ┌─────────────────────┐
  │   TF-IDF Engine     │
  │   Cosine Similarity │
  └──────────┬──────────┘
             │
             ▼
  ┌─────────────────────┐
  │   ICD-11 Matcher    │  ◀── WHO Standard Codes
  └──────────┬──────────┘
             │
             ▼
  ┌─────────────────────┐
  │   FHIR Output       │  ◀── Healthcare Interoperability
  └─────────────────────┘
```

- 🔍 Semantic search: TF-IDF + cosine similarity
- 🏥 FHIR-compliant structured output
- 🧩 Microservice architecture with REST APIs
- 🌐 Live and deployed on Render

[![View Repo](https://img.shields.io/badge/GitHub-Namaste--ICD11-0D1117?style=for-the-badge&logo=github&logoColor=white)](https://github.com/bhusareMayur/Namaste-ICD11)
[![Live Demo](https://img.shields.io/badge/Live_Demo-00C7B7?style=for-the-badge&logo=render&logoColor=white)](https://namaste-icd11.onrender.com)

</details>

---

## 🏗️ Currently Building

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=0,14,20&height=90&text=GoQueue%2B%2B&fontSize=48&fontColor=ffffff&fontAlign=50&desc=Distributed+Job+Processing+Engine+in+Go&descSize=16&descColor=c4b5fd&descAlign=50&animation=twinkling" width="80%"/>

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
    Observability []string // {"metrics", "traces", "structured_logs"}
    WorkerModel   string   // "goroutine pools + channels"
    FaultTolerant bool     // true — by design, not accident
}
```

<div align="center">

| Feature | Status |
|:---|:---:|
| 🔁 At-least-once delivery | 🔨 Building |
| 💀 Retry + Dead Letter Queue | 🔨 Building |
| 🛑 Worker crash recovery | 🔨 Building |
| 📊 Metrics + Structured Logs | 🔨 Building |
| ⚡ Goroutine worker pools | 🔨 Building |
| 🧪 Chaos & fault injection tests | 📋 Planned |

</div>

---

## 🧠 Engineering Principles

<div align="center">

```
┌─────────────────────────────────────────────────────────────────────┐
│                                                                     │
│   [reliability]                    [observability]                  │
│   expect_failure       = true      log_everything    = structured   │
│   design_for_recovery  = true      trace_distributed = true         │
│   idempotency_first    = true      alert_on_anomaly  = true         │
│                                                                     │
│   [architecture]                   [philosophy]                     │
│   decouple_with_queues = true      if_not_tested     = not_working  │
│   retry_transient      = true      build_for_recovery= not_perfection│
│   isolate_fault_zones  = true      failure           = expected     │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

</div>

---

<div align="center">

<br/>

*— Mayur Bhusare*

> **"Reliable systems are built by engineers who expect failure."**

<br/>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,50:4f46e5,100:7c3aed&height=130&section=footer"/>

</div>
