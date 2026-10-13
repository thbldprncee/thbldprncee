**Java Backend Developer** · **ITMO University** · **3rd-year Software Engineering student**

---

## 🚀 About Me

I'm a backend-focused Java developer interested in building reliable server-side systems, event-driven architecture, highload applications, and fintech products.

- 🎓 Software Engineering student at ITMO University
- 💻 Focused on Java, Spring Boot, PostgreSQL and distributed systems
- ⚡ Interested in highload systems, Kafka-based architecture and backend engineering
- 📍 Saint Petersburg

---

## 🛠 Tech Stack

### Backend
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Apache Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)

### Infrastructure & Tools
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

---

## 💼 Featured Projects

### 🔐 [FinGuard](https://github.com/thbldprncee/finguard)

**Real-time anti-fraud transaction monitoring system** — event-driven microservices for fintech-like transaction processing.

FinGuard simulates how financial platforms detect suspicious transactions in real time. Transactions are accepted through an API gateway, published to Kafka through a transactional outbox, scored by a rule-based fraud engine, and the decisions are streamed live to a React dashboard.

**Tech stack:** Java 21, Spring Boot, Spring Cloud Gateway, Kafka, PostgreSQL, Redis, Keycloak, React, TypeScript, Docker

**Key features:**
- Microservices communicating through Kafka, with a Transactional Outbox and idempotent consumers
- Concurrency-safe `Idempotency-Key` handling on the transaction API
- Fail-safe fraud rule engine: rule weights from the database, sliding-window velocity, structuring detection
- Decisions: `APPROVED`, `REVIEW_REQUIRED`, `BLOCKED`
- Keycloak (OIDC + PKCE) authentication, RS256 tokens validated by every service
- Kafka secured with SASL/SCRAM and per-service ACLs; one database per service
- Audit trail, notifications and a live SSE dashboard filtered per user

### 📝 [Formatted Text Converter](https://github.com/thbldprncee/formatted-text-converter)

**Text format converter built around a single immutable AST** — Markdown, XHTML, JSON, RTF, plain text and LaTeX.

Every input is parsed into one format-independent document model, so any format can be converted to any other, and operations like style removal are written once. The input format is recognised by content, the output format by file extension. All parsers (JSON, XML, RTF) are hand-written, with zero runtime dependencies.

**Tech stack:** Java 21, Gradle, Lombok, JUnit 5, AssertJ, JaCoCo, GitHub Actions

**Key features:**
- Sealed record AST with pattern matching and the Stream API
- Lossless round trips: Markdown → JSON / XHTML / RTF → Markdown is byte-identical
- Nested lists, tables, code blocks, links, images and quotes in every format
- Style removal, configurable indentation, document statistics
- Visitor, Strategy, Template Method, Builder and Facade; formats plug in via `ServiceLoader`
- 154 tests, 96% line coverage

---

## 📫 Contact

- 📧 Email: [thbldprnce@gmail.com](mailto:thbldprnce@gmail.com)
- 💬 Telegram: [@viennall](https://t.me/viennall)
