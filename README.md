<div align="center">

<!-- HEADER BANNER -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=200&section=header&text=Mayur%20Bhusare&fontSize=60&fontColor=ffffff&fontAlignY=38&desc=Backend%20%26%20Distributed%20Systems%20Engineer&descAlignY=58&descSize=20&descColor=a78bfa&animation=fadeIn" />

<!-- ANIMATED TYPING -->
<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=22&duration=2800&pause=900&color=A78BFA&center=true&vCenter=true&width=700&lines=⚙️+Distributed+Systems+%7C+Reliability+Engineering;🔁+Queue+Systems+%7C+Worker+Pools+%7C+DLQ;🐹+Building+GoQueue%2B%2B+in+Go;🛡️+Fault-Tolerant+%7C+At-Least-Once+Delivery;%22Reliable+systems+expect+failure.%22" alt="Typing SVG" />
</a>

<br/>

<!-- SOCIAL BADGES -->
<p>
  <a href="mailto:mayurbhusare8262@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-mayurbhusare8262-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
  <a href="YOUR_LINKEDIN_URL">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  <a href="YOUR_LEETCODE_URL">
    <img src="https://img.shields.io/badge/LeetCode-1665_Rating-FFA116?style=for-the-badge&logo=leetcode&logoColor=black"/>
  </a>
  <a href="YOUR_PORTFOLIO_URL">
    <img src="https://img.shields.io/badge/Portfolio-Visit_Now-a78bfa?style=for-the-badge&logo=firefox&logoColor=white"/>
  </a>
</p>

<img src="https://komarev.com/ghpvc/?username=bhusareMayur&color=a78bfa&style=flat-square&label=Profile+Views" />

</div>

---

<!-- ABOUT ME SECTION -->
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:0f0c29,100:302b63&height=3&section=header" width="100%"/>

<br/>

<table>
<tr>
<td valign="top" width="55%">

## 🧑‍💻 About Me

```yaml
name     : Mayur Bhusare
role     : Backend & Distributed Systems Engineer
location : India 🇮🇳
status   : Building GoQueue++ 🚀
passion  : Systems that survive real-world failure
```

I don't just write backend code — I **engineer reliability**.  
My obsession is understanding *why* systems fail and building the primitives that make them recover.

- 🔁 Deep in **queues, retries, DLQs, idempotency**
- 🐹 Mastering **Go** for concurrent, high-performance infra
- 📡 Heavy focus on **observability** and structured failure modes
- 🧠 **500+ DSA problems** · LeetCode Rating **1665**
- 🔬 Learning beyond coursework, always

</td>
<td valign="top" width="45%">

<br/>

<img src="https://raw.githubusercontent.com/platane/snk/output/github-contribution-grid-snake-dark.svg" width="100%" alt="contribution snake"/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=bhusareMayur&bg_color=0d1117&color=a78bfa&line=7c3aed&point=ffffff&area=true&hide_border=true" width="100%"/>

</td>
</tr>
</table>

---

<!-- TECH STACK -->
<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=24&height=50&text=⚡%20Tech%20Stack&fontSize=22&fontColor=ffffff&fontAlignY=70" width="100%"/>
</div>

<br/>

<div align="center">

**Languages**

<img src="https://skillicons.dev/icons?i=go,nodejs,js,python,java,cpp&theme=dark" />

**Backend & Messaging**

<img src="https://skillicons.dev/icons?i=express,rabbitmq,redis&theme=dark" />

**Databases & DevOps**

<img src="https://skillicons.dev/icons?i=mysql,mongodb,docker&theme=dark" />

**Testing & Tools**

<img src="https://skillicons.dev/icons?i=jest,git,github,linux&theme=dark" />

</div>

<br/>

---

<!-- PROJECTS SECTION -->
<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=24&height=50&text=🚀%20Featured%20Projects&fontSize=22&fontColor=ffffff&fontAlignY=70" width="100%"/>
</div>

<br/>

<!-- PROJECT 1 -->
<details open>
<summary>
  <b>🔥 &nbsp;Scalable Multi-Channel Notification System</b> &nbsp;
  <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white"/>
  <img src="https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white"/>
</summary>

<br/>

> **Async notification delivery at scale — Email · SMS · Push — engineered to survive burst traffic and worker crashes.**

```
                        ┌─────────────────────────────────────────┐
                        │         SYSTEM ARCHITECTURE             │
                        └─────────────────────────────────────────┘

  ┌──────────┐    ┌─────────────┐    ┌──────────────────┐    ┌──────────────┐
  │  Client  │───▶│  REST API   │───▶│   RabbitMQ       │───▶│ Worker Pool  │
  └──────────┘    └─────────────┘    │  Exchange/Queue  │    └──────┬───────┘
                                     └─────────────────-┘           │
                                              │                ┌─────▼──────┐
                                        Retry Queue ◀──────── │  Delivery  │
                                              │                │ Email/SMS/ │
                                         DLQ Handler           │   Push     │
                                              │                └────────────┘
                                       Structured Logs
```

<table>
<tr>
<td>

**⚙️ Engineering Features**
- ✅ Worker-based async processing
- ✅ Retry queues + Dead Letter Queue
- ✅ Idempotent consumers (no duplicates)
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
- Graceful degradation

</td>
</tr>
</table>

<br/>

[![View Repo](https://img.shields.io/badge/GitHub-notification--system-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/bhusareMayur/notification-system)

</details>

<br/>

<!-- PROJECT 2 -->
<details open>
<summary>
  <b>⚙️ &nbsp;resilient-queue — Open Source Redis Job Queue</b> &nbsp;
  <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white"/>
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white"/>
  <img src="https://img.shields.io/badge/Jest-C21325?style=flat-square&logo=jest&logoColor=white"/>
  <img src="https://img.shields.io/badge/Open_Source-❤️-ff6b6b?style=flat-square"/>
</summary>

<br/>

> **Redis-backed, fault-tolerant job queue with battle-hardened retry primitives.**

```
  Enqueue Job
      │
      ▼
  ┌───────────┐     ┌─────────────┐     ┌───────────────┐
  │  Redis    │────▶│   Worker    │────▶│   Execute     │
  │  LPUSH    │     │  (BLPOP)    │     │   Handler     │
  └───────────┘     └─────────────┘     └──────┬────────┘
                                               │
                                    ┌──────────┴──────────┐
                                    │                     │
                                ✅ Success            ❌ Failure
                                    │                     │
                                  Done         Exponential Backoff
                                                          │
                                                   Max Retries?
                                                  /            \
                                                No              Yes
                                                 │               │
                                            Retry Queue     💀 DLQ
```

- 🔂 Exponential backoff with jitter
- 🔑 Idempotency key support
- 💀 Dead Letter Queue for exhausted jobs
- 🛑 Graceful shutdown (drain before exit)
- ✅ Full Jest test coverage
- 🌍 Open-source contributor friendly

<br/>

[![View Repo](https://img.shields.io/badge/GitHub-resilient--queue-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/bhusareMayur/resilient-queue)

</details>

<br/>

<!-- PROJECT 3 -->
<details>
<summary>
  <b>🏥 &nbsp;NAMASTE ↔ ICD-11 Healthcare Mapping Platform</b> &nbsp;
  <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white"/>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/NLP-TF--IDF-blueviolet?style=flat-square"/>
  <img src="https://img.shields.io/badge/FHIR-Compliant-00897B?style=flat-square"/>
</summary>

<br/>

> **Bridging traditional medicine and global health standards through NLP and microservices.**

```
  Traditional Medicine Term
            │
            ▼
  ┌──────────────────────┐
  │   TF-IDF Engine      │  ◀── NLP Preprocessing
  │   Cosine Similarity  │
  └──────────┬───────────┘
             │
             ▼
  ┌──────────────────────┐
  │   ICD-11 Matcher     │  ◀── WHO Standard Codes
  └──────────┬───────────┘
             │
             ▼
  ┌──────────────────────┐
  │   FHIR Output        │  ◀── Healthcare Interoperability
  └──────────────────────┘
```

- 🔍 Semantic search with TF-IDF + cosine similarity
- 🏥 FHIR-compliant output format
- 🧩 Microservice architecture with REST APIs
- 🌐 Live demo deployed on Render

<br/>

[![View Repo](https://img.shields.io/badge/GitHub-Namaste--ICD11-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/bhusareMayur/Namaste-ICD11)
[![Live Demo](https://img.shields.io/badge/Live_Demo-namaste--icd11.onrender.com-00C7B7?style=for-the-badge&logo=render&logoColor=white)](https://namaste-icd11.onrender.com)

</details>

---

<!-- CURRENT BUILD -->
<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=24&height=50&text=🏗️%20Currently%20Building&fontSize=22&fontColor=ffffff&fontAlignY=70" width="100%"/>
</div>

<br/>

<div align="center">

```
╔══════════════════════════════════════════════════════════════════╗
║                                                                  ║
║   ██████╗  ██████╗  ██████╗ ██╗   ██╗███████╗██╗   ██╗███████╗ ║
║  ██╔════╝ ██╔═══██╗██╔═══██╗██║   ██║██╔════╝██║   ██║██╔════╝ ║
║  ██║  ███╗██║   ██║██║   ██║██║   ██║█████╗  ██║   ██║█████╗   ║
║  ██║   ██║██║   ██║██║▄▄ ██║██║   ██║██╔══╝  ██║   ██║██╔══╝   ║
║  ╚██████╔╝╚██████╔╝╚██████╔╝╚██████╔╝███████╗╚██████╔╝███████╗ ║
║   ╚═════╝  ╚═════╝  ╚══▀▀═╝  ╚═════╝ ╚══════╝ ╚═════╝ ╚══════╝ ║
║                           + +                                    ║
║          A Distributed Job Processing Engine in Go               ║
╚══════════════════════════════════════════════════════════════════╝
```

</div>

```go
// GoQueue++ — Engineered for production failure scenarios
type Engine struct {
    Language       string   // Go — concurrency-first
    Delivery       string   // "at-least-once"
    RetryPolicy    Backoff  // exponential with jitter
    DLQ            bool     // true — always
    CrashRecovery  bool     // true
    Observability  []string // {"metrics", "traces", "structured_logs"}
    WorkerModel    string   // "goroutine pools + channels"
    FaultTolerant  bool     // true — by design, not by accident
}
```

<div align="center">

| Feature | Status |
|---|---|
| 🔁 At-least-once delivery | 🔨 Building |
| 💀 Retry + DLQ | 🔨 Building |
| 🛑 Worker crash recovery | 🔨 Building |
| 📊 Observability (metrics + logs) | 🔨 Building |
| ⚡ Concurrent goroutine pools | 🔨 Building |
| 🧪 Chaos testing | 📋 Planned |

</div>

---

<!-- GITHUB STATS -->
<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=24&height=50&text=📊%20GitHub%20Stats&fontSize=22&fontColor=ffffff&fontAlignY=70" width="100%"/>
</div>

<br/>

<div align="center">

<img height="180" src="https://github-readme-stats.vercel.app/api?username=bhusareMayur&show_icons=true&theme=midnight-purple&hide_border=true&bg_color=0D1117&title_color=a78bfa&icon_color=a78bfa&text_color=ffffff&rank_icon=github&count_private=true" />
&nbsp;&nbsp;
<img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=bhusareMayur&layout=compact&theme=midnight-purple&hide_border=true&bg_color=0D1117&title_color=a78bfa&text_color=ffffff&langs_count=6" />

<br/><br/>

<img src="https://streak-stats.demolab.com?user=bhusareMayur&theme=midnight-purple&hide_border=true&background=0D1117&ring=a78bfa&fire=ff6b6b&currStreakLabel=a78bfa&sideLabels=a78bfa&dates=888888" />

</div>

---

<!-- PHILOSOPHY -->
<div align="center">

<br/>

```
┌────────────────────────────────────────────────────────────────────────┐
│                                                                        │
│    If it hasn't failed yet, you haven't tested it hard enough.         │
│    Build for recovery, not perfection.                                 │
│                                                                        │
│         "Reliable systems are built by engineers who expect failure."  │
│                                                          — Mayur       │
│                                                                        │
└────────────────────────────────────────────────────────────────────────┘
```

</div>

<!-- FOOTER WAVE -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:24243e,50:302b63,100:0f0c29&height=120&section=footer"/>
