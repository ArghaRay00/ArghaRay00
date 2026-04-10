### Hey, I'm Argha

Software engineer in Bangalore. Nine years of building backend systems that actually run in production — mostly at [Motorola Solutions](https://www.motorolasolutions.com/), where I work on the infrastructure behind their push-to-talk platform.

I care about systems that are reliable, codebases that are honest, and tools that make other people's work easier. I write Java, TypeScript, Python, and C# during the week. On nights and weekends, I build things that probably shouldn't exist but do anyway.

Lately I've been spending a lot of time thinking about agent engineering — the layer between AI models and the real world. How do you give an agent memory? How does it know when to speak and when to listen? How do you make it feel less like a chatbot and more like someone who actually knows you?

I don't have all the answers, but I'm building my way toward them.

[argha.dev](https://argha.dev) · [LinkedIn](https://www.linkedin.com/in/argha-ray/) · [X](https://x.com/argharay94)

---

### What I do at work

**Authorization & Access Control** — I own the RBAC microservice for Motorola's Kodiak platform. Java, Spring Boot, PostgreSQL. Role-permission management for their entire unified communications system. I wrote the test suite, refactored the service boundaries, and I'm the person people come to when something in the permission layer doesn't work right.

**PostgreSQL Infrastructure** — Currently helping architect a highly available PostgreSQL setup for storing 60TB of call recordings. Patroni for failover, pgEdge for cross-site replication, pgBackRest for backups. I'm building the tooling and running the proof of concept.

**Telecom Platform** — Before the current role, I spent three years on OnePortal — Motorola's multi-tenant provisioning portal. Full-stack across Angular and ASP.NET Core. Device management, carrier integrations across six MVNOs, Okta auth, webhook systems, certificate management. I joined the team knowing nothing about the codebase and ended up owning large parts of it.

**Device Cloud** — Worked on the serverless device management layer — TypeScript on AWS Lambda, IoT Core for MQTT device shadows, DynamoDB. Investigated a production outage where I traced the real root cause after the original analysis had been accepted for months.

**Internal tools** — I tend to build tools when I see friction. A Bash deployment tool that the team now uses daily. A Jira-to-Chat notification system. A workshop on agentic engineering that I ran for the team. Small things that add up.

---

### What I build outside work

**[Jishu](https://jishu.argha.dev/chat)** — My most ambitious side project. A personal AI agent that runs 24/7 on my VPS, talks to me on Telegram in romanized Bengali, and knows everything about my work and life.

It has a cognitive architecture inspired by Bengali cultural concepts — seven modes of engagement (*Shravan* for listening, *Adda* for casual conversation, *Mantrana* for counsel, *Anusandhan* for research, and more), emotional attunement that reads mood from text patterns, and a self-reflection journal where it reviews its own behavior.

It searches the web autonomously, writes daily reviews, compiles knowledge from raw sources, and learns from conversations other people have with it. The whole thing runs on a single ARM VPS behind a Cloudflare Tunnel. Stack: Python, FastAPI, SearXNG for self-hosted search.

There's a guest chat where you can [talk to Jishu](https://jishu.argha.dev/chat) about me. He's friendly.

**[Streaming platform](https://argha.dev/posts/streaming-video-on-a-zero-dollar-server)** — A TVOD platform for movie rentals. NestJS backend, React frontend, Shaka Player for HLS. Built two versions — self-hosted (zero cost) and Bunny Stream CDN (with per-segment token auth). The architecture was designed so swapping the delivery layer required zero changes to auth, sessions, or the player. I wrote about the journey on my blog.

**[OnlineExam](https://github.com/ArghaRay00/OnlineExam)** — An exam system I wrote in college in .NET Framework 4.5, then rewrote a decade later in .NET 9 with Clean Architecture. Mostly to see how far the ecosystem has come. It's come far.

---

### Things I've explored

I learn by building. Some of these are finished, some are half-done experiments, some are just me figuring out how something works:

- Distributed key-value store (Dynamo-style gossip protocol)
- Load balancer in C#
- Event deduplication system in Go + Redis
- Angular Module Federation for cross-domain auth
- Protocol Buffers in .NET + Angular
- Hyperledger Fabric ledger visualization
- Server-Sent Events for real-time push
- SOLID principles with before/after refactoring examples
- Various full-stack starters (MEAN, .NET, Express)

The repos are all here. Some are polished, most are learning artifacts. That's the point.

---

### Tech I use

**Languages** — Java, TypeScript, Python, C#, Bash, SQL. Others come and go.

**Backend** — Spring Boot, ASP.NET Core, NestJS, FastAPI, Entity Framework, TypeORM

**Data** — PostgreSQL, SQL Server, DynamoDB, Elasticsearch, Redis, MongoDB

**Cloud** — AWS (Lambda, IoT Core, S3, DynamoDB), Docker, Cloudflare, GitHub Actions

**Frontend** — Angular, React. I can build UIs but my heart is in the backend.

---

### Let's talk

I'm always happy to chat about backend systems, agent architecture, or whatever you're building. If something here caught your eye — reach out.

[argha.dev](https://argha.dev) · [LinkedIn](https://www.linkedin.com/in/argha-ray/) · [X](https://x.com/argharay94)
