### Hey, I'm Argha

Full-stack engineer with 9+ years building enterprise systems, internal tools, and side projects. Currently at **Motorola Solutions** working on authorization services, deployment automation, and telecom platforms.

I write Java, C#, TypeScript, Python, and Bash professionally. On weekends I build things in NestJS, React, Go, and whatever else catches my attention.

---

### Work — Motorola Solutions

**Authorization Service** — Java 17, Spring Boot, PostgreSQL
- Built the role-based permission system — 6 roles, 35+ resource types, 2-bit hex-encoded rulesets (7 operations per permission)
- Wrote the agency provisioning pipeline — JSON transformation utility that reads permission matrices and INSERTs into ROLES + PERMISSIONS tables with transaction management
- Created `KnJsonTransformationUtility`, `KnResourceTypeMapper` (36 resource type → integer code mappings), `KnPermissionDAO` (7 SELECT queries + MERGE, 19 params)
- Added isViewable/isEditable fields across the full stack — entity, DAO, DTO, service, with server-side filtering (returns null for non-viewable, 4 call sites with null checks)
- Wrote **666+ API integration tests** across 22 modules covering all 20 POST endpoints. Full auth matrix verification (6 roles x 35 resources = 210 cells). Input validation, pagination, concurrency, security, business logic, idempotency
- Fixed the Maven deploy pipeline — resolved invalid Spring Boot dependency version (3.5.4 doesn't exist), 10 PRs merged to restore CI/CD

**Universal JAR Deployer** — Bash, 2,100+ lines
- Built a deployment tool used by 28+ developers sharing test servers. Solves the coordination chaos of manual SCP + restart cycles that was costing ~250 developer-hours/week
- 14 commands: deploy, rollback, status, logs, diff, ssh, info, diag, check, lock, unlock, lock-status, history, list
- Per-user timestamped backups, auto-lock on deploy with TTL, health checks (URL or port-based) with auto-rollback on failure, dry-run mode, DGlogs application log support, multi-user detection, update check against shared directory
- Designed the incremental prompt architecture (9-step build sequence) so the entire tool is reproducible from scratch

**DeployBot** — Python, Flask, Cloud Run
- Designed a Google Chat deployment bot with interactive card UI, deployment locks, SSH executor via Paramiko jump chains, audit logging to Google Sheets. Proposed to replace the manual coordination overhead

**CAT Requests & Approvals** — Java, Spring Boot
- Built paginated list API for the Central Admin Tool — `GET /api/requests/list` with filtering, sorting, search across inbound approvals and outbound requests
- Created 6 new Java classes (DTOs, service layer, REST controller), designed the request expiration scheduler (Spring @Scheduled), wrote 18 unit tests across 3 test files
- Implemented external users API with server-side pagination (OFFSET/LIMIT/COUNT/LIKE in SQL), field mapping from AuthZ service entities to CAT DTOs, epoch-to-ISO timestamp conversion

**OnePortal** — Angular, ASP.NET Core, SQL Server
- Telecom management platform — 28 API controllers, 90+ entity models, Okta JWT+JWE auth, Salesforce/MVNO integrations across 6 carriers
- Worked on webhook design for contract lifecycle, module federation investigation for cross-domain cookie auth, Broadcast Channel API for inter-app communication
- Contributed to patent analysis — identified 7 patentable innovations including multi-zone device cloning with selective cross-association

**MOTOTRBO Device Management** — AWS Lambda, TypeScript, MQTT, DynamoDB
- Device cloud services — 64 Lambda functions, AWS IoT Core with MQTT topic routing, device shadow-based configuration sync, X.509 certificate generation
- Built Python scripts for CloudWatch log extraction by entity ID, subscriber status mapping, connection pool analysis dashboards

**Other work**
- Ran a **2-day Agentic Engineering workshop** for the team — context engineering, prompt patterns, MCP servers, custom agents, live coding, deployer demo
- Designed **15 Google Workspace Studio agent blueprints** — PR digest, incident triage, standup generator, Jira summarizer, smart inbox organizer, release notes generator
- Built an **AI/ML tooling pitch** with React dashboard showing 90%+ cost savings vs commercial APIs for 500 employees. Recommended Qwen 3.5 2B, evaluated Unsloth/LLaMA-Factory/vLLM/MLX
- Automated **Jira-to-Google Chat workflows** — real-time ticket field change notifications, missing Target End Date reports, team reassignment alerts (saving 2.5-5 hrs/week)
- Handled **production incidents** — SQL Server connection pool debugging, .NET 6 to 8 migration SSL issues, script bundling errors, JSON deserialization fixes

---

### Side projects

**[Streaming platform](https://globo.argha.dev)** — Currently building a TVOD streaming platform. NestJS + PostgreSQL backend, React frontend, HLS video playback via Shaka Player, reverse proxy architecture. Designed the full streaming pipeline including DRM strategy, CDN delivery, and content encoding.

**Other things I'm working on** — A systematic trading system for Indian equity markets, and an AR-based mobile app. Both in early stages.

---

### Experiments & deep dives

- **Legacy .NET modernization** — rewrote [OnlineExam](https://github.com/ArghaRay00/OnlineExam) from .NET Framework 4.5.1 (ASP.NET MVC 5, EF6, SQL Server, plaintext passwords, no DI) to .NET 9 (Clean Architecture, Carter, MediatR, EF Core 9, PostgreSQL, JWT, BCrypt, Serilog, Scalar). 17 entities consolidated to 11, zero tests to xUnit, GitHub Actions CI
- **Distributed key-value store** — designed from scratch, studied Dynamo-style gossip protocols
- **C# load balancer** — built a working implementation
- **Concurrent programming in C#** — async patterns, paginated web APIs, connection pool analysis
- **Angular Module Federation** — cross-domain cookie auth, dynamic remote loading, Broadcast Channel API for inter-app communication
- **Okta integration** — transitioned client-side to server-side auth in ASP.NET Core + Angular
- **Protocol Buffers** — implemented in .NET 6 API + Angular frontend
- **FLIPMed** — medical appointment booking app (early project)
- **Multi-platform cab booking PWA** — explored PWA patterns
- **Event deduplication system** — designed with Go + Redis
- **Cloudflare Workers**, **tscircuit**, **fine-tuning open-source LLMs** — ongoing exploration
- **Personal finance automation** — designing unified dashboard for PPF, PF, stocks, MF with automated signals

---

### GitHub projects

| Project | What | Tech |
|---------|------|------|
| [OnlineExam](https://github.com/ArghaRay00/OnlineExam) | Online exam system — modernized from .NET Framework 4.5.1 to .NET 9. Clean Architecture, Carter, MediatR, JWT, BCrypt, EF Core, PostgreSQL. 20+ REST endpoints. Original preserved in v1-legacy branch | .NET 9, EF Core 9, Carter, MediatR, PostgreSQL |
| [mean-auth-starter](https://github.com/ArghaRay00/mean-auth-starter) | Full-stack JWT auth — signup, login, route guards, interceptors, email | MongoDB, Express, Angular 6, Node.js |
| [dotnet-ecommerce-api](https://github.com/ArghaRay00/dotnet-ecommerce-api) | Product catalog API — Clean Architecture, seed data, Swagger | .NET 5, EF Core, SQLite |
| [home-warranty-dashboard](https://github.com/ArghaRay00/home-warranty-dashboard) | Warranty admin dashboard — Yelp vendor search, assignment workflow | Angular 8, Material, Azure .NET |
| [snake-and-ladder-csharp](https://github.com/ArghaRay00/snake-and-ladder-csharp) | LLD exercise — configurable board, chaining logic, queue-based turns | C#, .NET Core |
| [angular-sse-demo](https://github.com/ArghaRay00/angular-sse-demo) | Server-Sent Events — real-time push over plain HTTP | Angular 14, Node.js |
| [spring-mvc-rest-crud](https://github.com/ArghaRay00/spring-mvc-rest-crud) | REST API — DAO pattern, JDBC template, no Spring Boot, all manual config | Spring MVC, MySQL |
| [hyperledger-mortgage-ui](https://github.com/ArghaRay00/hyperledger-mortgage-ui) | Blockchain ledger viewer — 3 Hyperledger Fabric channels | Angular 5, Material |
| [mortgage-ledger-ui](https://github.com/ArghaRay00/mortgage-ledger-ui) | Static ledger visualization — 8-stage mortgage workflow | Angular 5, Material |
| [ionic-google-maps-poc](https://github.com/ArghaRay00/ionic-google-maps-poc) | Geolocation, place autocomplete, geocoding for mobile | Ionic 3, Google Maps API |
| [ExpenseManager](https://github.com/ArghaRay00/ExpenseManager) | Expense tracker — DI, repository pattern, antiforgery middleware | ASP.NET Core 2.1, EF Core |
| [node-mysql-scaffolding](https://github.com/ArghaRay00/node-mysql-scaffolding) | Backend boilerplate — JWT auth, auto-seeding | Node.js, Express, MySQL |
| [solid-principles-csharp](https://github.com/ArghaRay00/solid-principles-csharp) | SOLID principles — before/after refactoring examples | C#, .NET Core |
| [interview-notes](https://github.com/ArghaRay00/interview-notes) | 3,000+ lines of DSA heuristics, patterns, problem-solving strategies | Markdown |

---

### Tech

**Languages** — Java, C#, TypeScript, JavaScript, Python, Bash, Go, Kotlin, SQL

**Backend** — Spring Boot, ASP.NET Core 9, ASP.NET MVC 5, NestJS, Express, Entity Framework (6 + Core 9), TypeORM, Spring JDBC, Carter, MediatR

**Frontend** — Angular (5–19), React 19, Ionic, Tailwind, Angular Material, RxJS

**Data** — PostgreSQL, MongoDB, MySQL, SQL Server, SQLite, DynamoDB, Redis, Elasticsearch

**Cloud** — AWS (Lambda, IoT Core, CloudWatch, S3, EC2, API Gateway, DynamoDB), Azure DevOps

**Infra** — Docker, Podman, Nginx, Serverless Framework, Cloudflare Workers

**Auth** — JWT, Okta (JWT+JWE), Passport.js, bcrypt, RBAC, X.509 certificates

**AI/ML** — Claude API, Qwen, vLLM, MLX, Unsloth, LLaMA-Factory, ARCore, ML Kit

**Tools** — Git, Maven, npm, Webpack, Module Federation, Protocol Buffers, Swagger/Scalar, Hangfire, Serilog, FluentValidation, GitHub Actions
