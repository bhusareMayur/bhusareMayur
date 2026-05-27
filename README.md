<div align="center">

```
╔╗ ╔═╗╔═╗╦╔═╔═╗╔╗╔╔╦╗
╠╩╗╠═╣║  ╠╩╗║╣ ║║║ ║║
╚═╝╩ ╩╚═╝╩ ╩╚═╝╝╚╝═╩╝
╔╦╗╔═╗╦ ╦╦ ╦╦═╗
║║║╠═╣╚╦╝║ ║╠╦╝
╩ ╩╩ ╩ ╩ ╚═╝╩╚═  BHUSARE
```

**`Backend & Distributed Systems Engineer`**

*Building systems that don't just work — they survive.*

</div>

<br/>

---

## ❯ whoami

```yaml
name     :  Mayur Bhusare
role     :  Backend & Distributed Systems Engineer
core     :  Reliability · Scalability · Fault Tolerance
building :  GoQueue++ — distributed job engine in Go
location :  India
email    :  mayurbhusare8262@gmail.com
```

I'm a Computer Engineering student who builds systems beyond standard coursework —
focused on **what happens when things fail** and **how they recover.**

```
Things I think about at 2am:
  ├── Will this worker recover if it crashes mid-job?
  ├── What if the queue gets flooded?
  ├── Is this delivery truly idempotent?
  └── Can I observe the failure before the user does?
```

---

## ❯ cat tech-stack.txt

```
┌────────────────────────────────────────────────────────────────┐
│  LANGUAGES       Go · Node.js · JavaScript · Python · Java · C++ │
│  BACKEND         Express.js · REST APIs                         │
│  MESSAGING       RabbitMQ · Redis                               │
│  DATABASES       MySQL · MongoDB                                │
│  INFRA           Docker · k6                                    │
│  TESTING         Jest                                           │
└────────────────────────────────────────────────────────────────┘
```

---

## ❯ ls -la projects/

<br/>

### 🔥 &nbsp; Scalable Multi-Channel Notification System
> *Async notification delivery — Email, SMS, Push — built for real-world failure.*

```
  CLIENT REQUEST
       │
       ▼
  ┌─────────┐       ┌───────────┐      ┌──────────────────┐
  │  API    │──────▶│ RabbitMQ  │─────▶│  Worker Pool     │
  │  Layer  │       │  Exchange │      │  (Horizontal)    │
  └─────────┘       └───────────┘      └────────┬─────────┘
                          │                     │
                    ┌─────┘               ┌─────▼──────┐
                    │                     │  Channels  │
               ┌────▼─────┐              ├────────────┤
               │  Retry   │              │ ✉  Email   │
               │  Queue   │              │ 📱 SMS     │
               └────┬─────┘              │ 🔔 Push    │
                    │                     └────────────┘
               ┌────▼─────┐
               │   DLQ    │  ◀── exhausted retries land here
               └──────────┘
```

| Concept | Implementation |
|---|---|
| Delivery Guarantee | At-least-once semantics |
| Retry Strategy | Exponential backoff + Dead Letter Queue |
| Duplicate Prevention | Idempotent consumers |
| Failure Visibility | Structured logging on every retry |
| Scalability | Horizontal worker scaling |
| Load Testing | k6 burst traffic simulation |

**`Node.js`** **`RabbitMQ`** **`Docker`** **`MySQL`** **`k6`**
&nbsp;&nbsp; → &nbsp; [github.com/bhusareMayur/notification-system](https://github.com/bhusareMayur/notification-system)

<br/>

---

### ⚙️ &nbsp; resilient-queue &nbsp;·&nbsp; Open Source
> *A Redis-backed job queue built around the primitives that actually matter.*

```
  ENQUEUE JOB
      │
      ▼
  ┌───────────────────────────────────────────────────┐
  │  Redis List  ◀──  BLPOP (blocking pop, no polling) │
  └───────────────────────────────┬───────────────────┘
                                  │
                            ┌─────▼──────┐
                            │  Execute   │
                            └─────┬──────┘
                       ┌──────────┴──────────┐
                       ▼                     ▼
                   ✅ Success           ❌ Failure
                                            │
                                   Exponential Backoff
                                            │
                                  ┌─────────▼─────────┐
                                  │  attempts < max?  │
                                  └────┬──────────┬───┘
                                      YES         NO
                                       │           │
                                  Retry Queue   Dead Letter Queue
```

- Exponential backoff with jitter
- Dead Letter Queue for exhausted jobs
- Idempotency key enforcement
- Graceful shutdown — no job left mid-flight
- Full Jest test coverage

**`Node.js`** **`Redis`** **`BLPOP`** **`Jest`**
&nbsp;&nbsp; → &nbsp; [github.com/bhusareMayur/resilient-queue](https://github.com/bhusareMayur/resilient-queue)

<br/>

---

### 🏥 &nbsp; NAMASTE ↔ ICD-11 Mapping Platform
> *Bridging traditional medicine and global health standards through NLP.*

```
  NAMASTE Term Input
         │
         ▼
  ┌──────────────────┐     ┌────────────────────┐
  │  TF-IDF Engine   │────▶│  Cosine Similarity  │
  └──────────────────┘     └─────────┬──────────┘
                                     │
                              ┌──────▼──────┐
                              │  ICD-11     │
                              │  Code Match │
                              └──────┬──────┘
                                     │
                              ┌──────▼──────┐
                              │  FHIR       │
                              │  Output     │
                              └─────────────┘
```

**`Node.js`** **`Python`** **`NLP`** **`FHIR`**
&nbsp;&nbsp; → &nbsp; [github.com/bhusareMayur/Namaste-ICD11](https://github.com/bhusareMayur/Namaste-ICD11)
&nbsp;&nbsp; → &nbsp; [namaste-icd11.onrender.com](https://namaste-icd11.onrender.com)

---

## ❯ top -p GoQueue++

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  PROCESS   GoQueue++                STATUS   🔨 BUILDING
  LANGUAGE  Go                       CPU      ████████ 100%
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

A distributed job processing engine in Go — built from scratch.

```go
type GoQueueEngine struct {
    Delivery        DeliveryMode  // AtLeastOnce
    RetryPolicy     BackoffPolicy // Exponential + Jitter
    DLQ             bool          // true
    WorkerPool      Concurrency   // goroutines + channels
    CrashRecovery   bool          // true
    Observability   []Signal      // Metrics, Traces, Logs
    FaultTolerance  bool          // always true
}
```

```
  ROADMAP
  ├── [✅] Worker pool with goroutines
  ├── [✅] At-least-once delivery
  ├── [✅] Exponential backoff + DLQ
  ├── [🔨] Crash recovery & state persistence
  ├── [🔨] Distributed worker coordination
  └── [⏳] Prometheus metrics + trace spans
```

---

## ❯ cat engineering.principles

```ini
; How I think about systems

[reliability]
expect_failure          = true
design_for_recovery     = true
idempotency_first       = true
no_silent_failures      = true

[architecture]
decouple_via_queues     = true
retry_transient_errors  = true
isolate_fault_domains   = true
horizontal_over_vertical = true

[observability]
log_format              = structured
trace_distributed_calls = true
measure_before_optimize = true

[problem_solving]
leetcode_rating         = 1665
dsa_problems_solved     = 500+
preferred_area          = system_design + backend
```

---

## ❯ ping mayur

```
  📌  LinkedIn    →  YOUR_LINKEDIN_URL
  🌐  Portfolio   →  YOUR_PORTFOLIO_URL
  🧠  LeetCode    →  YOUR_LEETCODE_URL   (Rating: 1665)
  📬  Email       →  mayurbhusare8262@gmail.com
```

---

<div align="center">

```
╔══════════════════════════════════════════════════════════════════╗
║                                                                  ║
║    "Reliable systems are built by engineers who expect failure." ║
║                                                                  ║
║                                             — Mayur Bhusare      ║
╚══════════════════════════════════════════════════════════════════╝
```

</div>
