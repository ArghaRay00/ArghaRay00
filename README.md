### Hey, I'm Argha

Software engineer in Bangalore. Nine years of building backend systems that actually run in production — mostly at [Motorola Solutions](https://www.motorolasolutions.com/), where I work on the infrastructure behind their push-to-talk platform.

I care about systems that are reliable, codebases that are honest, and tools that make other people's work easier. I write Java, TypeScript, Python, and C# during the week. On nights and weekends, I build things that probably shouldn't exist but do anyway.

Lately I've been deep into agent engineering — the layer between AI models and the real world. How do you give an agent memory? How does it know when to speak and when to listen? I'm building my way toward answers.

[argha.dev](https://argha.dev) · [LinkedIn](https://www.linkedin.com/in/argha-ray/) · [X](https://x.com/argharay94)

---

### What I do at work

**Authorization & Access Control** · Java, Spring Boot, PostgreSQL — Own the RBAC microservice for Motorola's Kodiak platform. Six roles, thirty-five resource types, hex-encoded permission bitmasks. Wrote the integration test suite, refactored the monolith, built the cross-service integration with [CAT](https://waveoncloud.com/).

**PostgreSQL Infrastructure** · Python, Patroni, pgEdge, pgBackRest — Helping architect a highly available PostgreSQL backend for 60TB of call recordings. Built a Python wrapper for pgBackRest with monitoring and benchmarking. Running the PoC.

**Kaiser Program** · ASP.NET Core, C#, TypeScript, AWS Lambda, IoT Core — Built WiFi Enterprise certificate management end to end across two repos (OnePortal + Device Cloud Services). Database schema design, S3 storage, certificate lifecycle APIs, IoT topic rules for device-side distribution. Biggest feature I shipped in 2025.

**Telecom Platform (OnePortal)** · Angular 5→19, ASP.NET Core, SQL Server, AWS — Three years full-stack on Motorola's multi-tenant provisioning portal. Device cloning, carrier transition (Telna → WirelessLogic), webhook integrations, gateway management, notification center, license renewal webhooks, Mototrbo R7 DualMode device support, reseller bulk operations, EVA token authentication, .NET 5→8 migration. Identified seven patent candidates through IPR analysis.

**Device Cloud Services** · TypeScript, AWS Lambda, IoT Core, DynamoDB — Serverless device management layer. Built Lambda handlers for Kaiser certificate distribution, production config rollouts. Independently reinvestigated a major outage and corrected the accepted root cause analysis.

**Internal tools** — A Bash deployment tool the team uses daily (20+ commands, health checks, auto-rollback, golden image management). A Jira-to-Chat notification system. Designed an AYT analytics config service (Java 21, HANA, Kafka). Ran a two-day agentic engineering workshop for the team.

---

### What I build outside work

**[Vesper](https://vesper.argha.dev/chat)** — A 24/7 personal AI agent on my VPS. Talks to me on Telegram in romanized Bengali. Has a cognitive architecture with three layers — core identity (soul, dharma, voice), perception (emotional attunement, life seasons, text signal reading), and cognition (seven Bengali modes of engagement: *Shravan*, *Adda*, *Mantrana*, *Jigyasa*, *Anusandhan*, *Utsav*, *Satarka*).

Searches the web autonomously via self-hosted SearXNG, writes daily reviews, compiles wiki pages from raw sources, learns from guest conversations. [Talk to her](https://vesper.argha.dev/chat) — she's friendly.

Stack: Python, FastAPI, SearXNG, APScheduler, Groq Whisper, GitHub Actions CI/CD. Runs on an Oracle ARM VPS behind Cloudflare Tunnel.

**[Streaming platform](https://argha.dev/posts/streaming-video-on-a-zero-dollar-server)** — TVOD movie rental platform. NestJS + React + Shaka Player. Two versions — self-hosted HLS (zero cost) and Bunny Stream CDN (per-segment token auth via Shaka's network engine). Swapping the delivery layer required zero changes to auth, sessions, or the player.

**PrepForge** — Interview prep system. 3,000+ DSA problems with company-wise tagging, system design scenarios, OOD problems. FSRS spaced repetition to surface problems based on forgetting curves. Python + FastAPI + React + SQLite.

**[OnlineExam](https://github.com/ArghaRay00/OnlineExam)** — Exam system I wrote in college (.NET Framework 4.5), rewrote a decade later in .NET 9 with Clean Architecture. Carter, MediatR, EF Core 9, xUnit, GitHub Actions CI.

---

### Things I've explored

I learn by building. Some finished, some half-done, some just me figuring out how something works:

- Distributed key-value store (Dynamo-style gossip protocol)
- Load balancer in C#
- Event deduplication in Go + Redis
- Angular Module Federation for cross-domain auth
- Protocol Buffers in .NET + Angular
- Hyperledger Fabric ledger visualization
- Server-Sent Events for real-time push
- SOLID principles with before/after refactoring

The repos are all here. Some are polished, most are learning artifacts. That's the point.

---

### Tech

**Languages** — Java, TypeScript, Python, C#, Bash, SQL

**Backend** — Spring Boot, ASP.NET Core, NestJS, FastAPI, Entity Framework, TypeORM

**Data** — PostgreSQL, SQL Server, DynamoDB, Elasticsearch, Redis

**Cloud** — AWS (Lambda, IoT Core, S3, DynamoDB), Docker, Cloudflare, GitHub Actions

**Frontend** — Angular, React — I can build UIs but my heart is in the backend

---

### Let's talk

I'm always happy to chat about backend systems, agent architecture, or whatever you're building. The full story is at [argha.dev/about](https://argha.dev/about).

[argha.dev](https://argha.dev) · [LinkedIn](https://www.linkedin.com/in/argha-ray/) · [X](https://x.com/argharay94)
