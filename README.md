<div align="center">

# Ashenafi Alemu

### Senior Backend Engineer · Go · Payments • Crypto • iGaming

🇪🇹 Addis Ababa, Ethiopia · Available for senior roles & consulting engagements

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ashenafi-alemu-%F0%9F%87%AA%F0%9F%87%B9-627b44155/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Ashenafi-pixel)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ashenafialemu27@gmail.com)

</div>

---

## 🎯 What I do

I build the backends that move money and run games.

Currently architecting a multi-tenant **iGaming platform at [GameCrafter](https://github.com/gamecrafter-io)** — a Remote Gaming Server with cryptographically verifiable fairness, sub-50ms real-time, and per-operator transaction routing. The goal: surpass SoftSwiss and EveryMatrix on latency, transparency, and developer ergonomics.

Before that, I shipped production payment infrastructure across **AddisPay** and **LakiPay** (Ethiopian rails) and built multi-currency wallet + KYC + bonus systems for LATAM operators serving 100k+ users.

---

## 🛠 Stack

<div align="center">

![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Apache Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![ClickHouse](https://img.shields.io/badge/ClickHouse-FFCC01?style=for-the-badge&logo=clickhouse&logoColor=black)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![gRPC](https://img.shields.io/badge/gRPC-244C5A?style=for-the-badge&logo=grpc&logoColor=white)

</div>

| Area | Tools & approaches |
|------|--------------------|
| **Languages** | Go (primary), Python, PHP, JavaScript |
| **Data** | PostgreSQL · ClickHouse · Redis · Supabase |
| **Streaming** | Kafka · Redis Pub/Sub · Event sourcing · CDC |
| **Cloud & Infra** | AWS (ECS, S3, RDS, Lambda) · Cloudflare · Docker · Kubernetes |
| **APIs** | REST · gRPC · WebSocket · WebTransport (HTTP/3) |
| **Observability** | Prometheus · Grafana · OpenTelemetry · Loki |
| **Cryptography** | SHA-256 commit-reveal · HMAC draws · On-chain anchoring · NIST SP 800-90A DRBG |
| **Patterns** | Multi-tenant isolation · Actor-per-room · Circuit breakers · Idempotency · CQRS |

---

## 🚀 Selected work

### 🎰 GameCrafter — Multi-Tenant Remote Gaming Server
> Multi-operator RGS in Go: per-operator transaction routing, S3-backed game asset delivery, Kafka-driven event sourcing, provably-fair draw engine. Designed to compete with SoftSwiss/EveryMatrix on latency and verifiable fairness.

**Highlights:**
- Per-operator request routing with circuit breakers + per-tenant observability
- HTTP/3 + WebTransport-first real-time protocol with WebSocket fallback
- Commit-reveal fairness with daily Merkle anchoring to Bitcoin + Ethereum (industry first)
- 96-game catalogue, 3 operators in production, deterministic round replay

### 💳 Integra P2P Payment Webhook
> Ingests bank P2P payment notifications from Venezuelan rails, idempotently credits the right player wallet, fires Kafka events for downstream analytics + RG monitoring.

**Highlights:**
- Idempotency by `referencia` (X-Trace-ID changes per retry per spec)
- 5-strategy user resolution from free-text `concepto` field
- Atomic balance update + audit log + Kafka publish in single transaction
- Kafka-based fan-out to fraud detection + CRM + regulator streaming

### 🎮 Raffle Multiplayer (Cryptographically Verifiable)
> Multi-player raffle game where any player can mathematically verify the round was fair. Combines commit-reveal with HMAC over all submitted tickets so the server can't pick the seed after seeing tickets.

**Highlights:**
- Per-round `SHA-256(seed ‖ round_id)` commitment
- `HMAC-SHA256(seed, canonical_tickets)` deterministic draw
- Daily Merkle root anchored to Bitcoin + Ethereum mainnet
- Player-side CLI verification tool

### 🏗 Multi-Operator Casino Platform
> JuegaEnTuCasino + ApuestasX live; Supabase → AWS PostgreSQL migration; multi-currency wallet, KYC hooks, bonus engine groundwork, responsible-gaming controls.

### 💸 AddisPay & LakiPay (Ethiopian Payment Gateways)
> Card processing, settlement, reconciliation, and webhook delivery for fintech rails serving local merchants and remittance flows.

---

## 📊 GitHub Activity

<div align="center">

![Stats](https://github-readme-stats.vercel.app/api?username=Ashenafi-pixel&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=Ashenafi-pixel&layout=compact&theme=tokyonight&hide_border=true&langs_count=8)

![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=Ashenafi-pixel&theme=tokyonight&hide_border=true)

</div>

---

## 💡 What I'm good at

- **Go backends that hold up under production load** — connection pooling, graceful degradation, observability built-in from day one
- **Payment integrations done right** — idempotency, reconciliation, retries, signed webhooks; the boring stuff that decides whether money is lost or not
- **Multi-tenant SaaS architecture** — per-tenant isolation, circuit breakers, rate limits, observability tagging end-to-end
- **Event-driven systems** — Kafka producers/consumers, event sourcing, deterministic replay, CDC pipelines
- **Cryptographic protocol design** — commit-reveal, HMAC constructions, public-chain anchoring for verifiability
- **Production debugging** — reading dashboards, tracing distributed flows, finding the one bad row in 100M

---

## 📬 Let's talk

I'm open to:

- 🎰 **iGaming / crypto-casino platform engagements** — RGS architecture, multi-tenant routing, fairness protocols, regulatory compliance
- 💳 **Payment-gateway integration consulting** — Ethiopian + LATAM rails, reconciliation, webhook reliability
- 🏗 **Senior Backend Engineer (Go) roles** — payments, gaming, fintech, marketplaces
- 🔧 **Technical architecture review** — multi-tenant Go backends, event-driven systems, real-time services

<div align="center">

[![LinkedIn](https://img.shields.io/badge/Connect_on_LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ashenafi-alemu-%F0%9F%87%AA%F0%9F%87%B9-627b44155/)
[![Email](https://img.shields.io/badge/Email_me-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:ashenafialemu27@gmail.com)

</div>

---

<div align="center">

*"The boring infrastructure underneath is where I do my best work."*

⭐ If something here is useful to you, a star on a relevant repo means a lot.

</div>
