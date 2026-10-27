<div align="center">

<img src="https://avatars.githubusercontent.com/u/80452645?v=4" width="150" style="border-radius:50%" alt="Kien Nguyen" />

# Hi, I'm Kien Nguyen 👋

### Tech Lead · Backend & Integrations · Travel-tech · Hanoi, Vietnam 🇻🇳

*I connect travel companies to the world's hotel, flight, tour and transfer suppliers — and keep those connections fast, correct and boring in production.*

<a href="https://kiennguyen2k1.vn"><img src="https://img.shields.io/badge/portfolio-kiennguyen2k1.vn-0A66C2?style=for-the-badge" /></a>
<a href="https://linkedin.com/in/kien-nguyen-178980256"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
<a href="mailto:nguyenkien2022001@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
<a href="https://gitlab.com/Trungkien2022001"><img src="https://img.shields.io/badge/GitLab-FC6D26?style=for-the-badge&logo=gitlab&logoColor=white" /></a>

![Profile views](https://komarev.com/ghpvc/?username=Trungkien2022001&color=0A66C2&style=flat-square)

</div>

---

## 🙋 About me

- 🎓 **B.Sc. in Computer Science — Hanoi University of Science and Technology (HUST)**.
- 🏨 I spend my days inside **B2B travel distribution** — the plumbing between agencies / airlines / OTAs and the suppliers that actually hold the inventory.
- 🔌 My speciality is **supplier integration**: reading someone else's REST / SOAP / XML API, finding its quirks, and turning it into one clean, predictable contract.
- 🧮 I care about the boring-but-expensive details: **multi-room pricing, cancellation deadlines and time zones, currency, idempotent cancels, retries** — the things that cost real money when they're wrong.
- 🗺️ I enjoy **data matching problems** — hundreds of thousands of hotels, five different naming conventions, GPS that's "close enough".
- 🤖 Lately I build **AI-assisted engineering & ops tooling**: agents that triage partner chat, investigate bookings from logs, and ship small fixes behind review gates.
- 💬 Vietnamese (native) · English (daily work with partners in Europe, Middle East, India and SEA).

---

## 💼 Experience

### 🏢 easyGDS / Altovo — Tech Lead, Hotel Gateway & Integrations *(current)*
B2B travel gateway serving travel agencies, airline holiday platforms and B2B resellers.

**Hotel gateway (offer-worker + booking-api)**
- Tech lead of the hotel aggregation service — own architecture, supplier roadmap, code review and production on-call: one **search → getrooms → prebook → book → retrieve → cancel** API over **40+ suppliers**.
- Stack: **Node.js · Koa · MySQL (Knex) · Redis · AWS SQS workers · Datadog / Grafana / Loki / Sentry**.
- Led / contributed to the **V2 → V3 architecture migration** (20+ suppliers in ~2 weeks): offer-centric response, pluggable "direct-offer" vs "matrix" pricing patterns, unified cancellation-policy normalisation.
- **SearchV3 performance work** — worker write-path, caching layout, payload compression, chunked supplier fan-out.

**Supplier integrations shipped (selection)**

| Area | Suppliers / platforms |
|---|---|
| Juniper ecosystem | Juniper DMCs (Roibos, W2M, EET, PeakPoint, Escalabeds…) — one module, many accounts |
| Wholesalers / bedbanks | DOTW / WebBeds (v4), Hotelbeds APItude, RateHawk, Hotelston, TBO, Miki, Illusions |
| Direct / chain | **Jumeirah Direct Connect**, Rakuten Travel Xchange (RTX), Amadeus, Travelport (demo) |
| Asia-Pacific | Accomy (incl. V2 → Open Platform V3 migration), Ottila / XConnect (APIOUT v2), Nuitee, HyperGuest |
| Hubs | TravelHub v1/v2 adapters (Jumeirah, Accomy) |

For each: API study → adapter → mapping → certification with the partner → go-live → on-call.

**Hotel content mapping**
- Built the matching pipeline that maps supplier catalogues to our inventory: **GIATA multi-codes + GPS distance + name / address / zip / star / chain scoring**, validated against known mappings (**~99.8% precision**).
- Examples: Hotelston **~650k** properties mapped, Rakuten **~270k**, large Juniper / Hilton portfolio audits.

**Reliability & ops**
- Distributed tracing design (Sentry sampling, supplier fan-out as child spans), Grafana dashboards & alerts, Loki log forensics.
- GitLab CI/CD with gated prod deploys, post-deploy monitoring and rollback.
- Partner-facing support: booking investigations, certification test suites, IP whitelisting, credential rotation.

**Also**: flight gateway (Amadeus / 1A flows), tour & transfer gateways, car-hire replay tooling.

### 🏢 VNTrip — Software Engineer
- **EMS** (expense / purchase-order management): multi-level approval workflows, notifications, FE + BE (React + NestJS).
- **Flight checkout & delay insurance** (PVI DelayCare): insurance lifecycle, polling / webhooks, reconciliation against flight segments.
- Internal tooling: E2E test suites, reporting, Mattermost integrations.

### 🎓 Hanoi University of Science and Technology (HUST)
- **Bachelor of Computer Science** — graduated.

---

## 🛠️ Tech stack

**Languages** &nbsp;
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

**Backend** &nbsp;
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![Koa](https://img.shields.io/badge/Koa-33333D?style=flat-square&logo=koa&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![Spring](https://img.shields.io/badge/Spring-6DB33F?style=flat-square&logo=spring&logoColor=white)
![SOAP/XML](https://img.shields.io/badge/SOAP%20%2F%20XML-555555?style=flat-square)
![REST](https://img.shields.io/badge/REST-02569B?style=flat-square)

**Data & messaging** &nbsp;
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Elasticsearch](https://img.shields.io/badge/Elasticsearch-005571?style=flat-square&logo=elasticsearch&logoColor=white)
![ClickHouse](https://img.shields.io/badge/ClickHouse-FFCC01?style=flat-square&logo=clickhouse&logoColor=black)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white)
![BullMQ](https://img.shields.io/badge/BullMQ-E8352E?style=flat-square)
![AWS SQS](https://img.shields.io/badge/AWS_SQS-FF4F8B?style=flat-square&logo=amazonsqs&logoColor=white)

**Frontend** &nbsp;
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Redux](https://img.shields.io/badge/Redux-764ABC?style=flat-square&logo=redux&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)

**Cloud, CI/CD & observability** &nbsp;
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![GitLab CI](https://img.shields.io/badge/GitLab_CI-FC6D26?style=flat-square&logo=gitlab&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![Loki](https://img.shields.io/badge/Loki-F46800?style=flat-square&logo=grafana&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Sentry](https://img.shields.io/badge/Sentry-362D59?style=flat-square&logo=sentry&logoColor=white)
![Datadog](https://img.shields.io/badge/Datadog-632CA6?style=flat-square&logo=datadog&logoColor=white)

**Testing & tooling** &nbsp;
![Jest](https://img.shields.io/badge/Jest-C21325?style=flat-square&logo=jest&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white)
![Claude](https://img.shields.io/badge/Claude_Code-D97757?style=flat-square&logo=anthropic&logoColor=white)

---

## 🏗️ How a hotel search flows through what I build

```text
 Agency / OTA / airline site
            │  POST /search  (destination or hotel ids, rooms, dates)
            ▼
 ┌─────────────────────────┐     fan-out per supplier     ┌──────────────────────┐
 │  Gateway API (Koa)      │ ───── SQS jobs ────────────▶ │  Workers             │
 │  auth · validation      │                              │  supplier adapters   │
 │  mapping (hotel ↔ code) │ ◀──── Redis offers ───────── │  REST / SOAP / XML   │
 └─────────────────────────┘                              └──────────┬───────────┘
            │ getrooms / search-by-id                                 │
            ▼                                                         ▼
   prebook (re-price, policy) ──▶ book ──▶ retrieve / cancel   40+ hotel suppliers
```

- **Two pricing patterns**: *direct-offer* (supplier returns one token for N rooms) vs *matrix* (independent per-room rates combined by us).
- **One cancellation model**: every supplier's policy normalised to `{from, to, amount, timezone}`, merged per offer, deadlines in UTC.
- **Mapping layer**: supplier hotel codes ↔ our hotel ids, cached and flushed per hotel / region.

---

## 📈 Numbers I'm proud of

| | |
|---|---|
| 🔌 Hotel suppliers integrated / maintained | **40+** |
| 🗺️ Hotels mapped for a single supplier | **~650,000** |
| 🎯 Mapping precision on known ground truth | **~99.8%** |
| ⚡ V2 → V3 supplier migration | **20+ suppliers in ~2 weeks** |
| ✅ Partner certifications passed | Juniper DMCs, RTX, Hotelston, Jumeirah, … |

---

## 📌 Public projects

| Project | Stack | What it is |
|---|---|---|
| [vtravel](https://github.com/Trungkien2022001/vtravel) | NestJS · TypeScript | Travel booking backend — search, booking, payments |
| [vtravel-client](https://github.com/Trungkien2022001/vtravel-client) | React · TypeScript | Client for vtravel |
| [vnt-sdk](https://github.com/Trungkien2022001/vnt-sdk) | TypeScript | SDK wrapping a travel API |
| [auction](https://github.com/Trungkien2022001/auction) | Node.js · React | Real-time online auction system |
| [english_app](https://github.com/Trungkien2022001/english_app) | TypeScript | English learning app |
| [kien-nguyen-support](https://github.com/Trungkien2022001/kien-nguyen-support) | JavaScript | Personal tooling & support scripts |

Most of my day-to-day work lives in private company repositories.

---

## 🌱 Currently

- 🏗️ Migrating suppliers to new API versions (Accomy Open Platform V3, Ottila APIOUT v2)
- 🔭 End-to-end tracing across the gateway (Sentry) — supplier calls as child spans of the search
- 🤖 Building AI agents for integration support & on-call
- 📚 Learning: distributed systems design, Go, better ways to test third-party integrations

## 🤝 Open to

Talking about **travel-tech APIs, supplier integrations, hotel mapping, and backend performance**. Happy to help with tricky supplier docs — I've read a lot of them.

---

## 📊 GitHub stats

<div align="center">
<img height="165" src="https://github-readme-stats.vercel.app/api?username=Trungkien2022001&show_icons=true&count_private=true&hide_border=true&theme=default" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Trungkien2022001&layout=compact&hide_border=true" />
<br/>
<img src="https://streak-stats.demolab.com?user=Trungkien2022001&hide_border=true" height="165" />
</div>

---

<div align="center">

🎓 B.Sc. Computer Science · Hanoi University of Science and Technology (HUST)

*"Make the integration boring. Boring is reliable."*

</div>
