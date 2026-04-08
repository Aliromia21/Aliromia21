# Ali Romia

**Backend & Full-Stack Engineer** — building distributed systems, real-time pipelines, and production-grade APIs.  
M.Sc. Computer Science at TU Braunschweig · Based in Hannover, Germany.

---

## What I Build

I design and build backend systems that process data at scale — event streaming with Kafka, real-time dashboards with WebSockets, and production APIs with testing and CI/CD. I care about architecture decisions, not just code that works.

---

## Featured Projects

### [ThreatStream](https://github.com/Aliromia21/threatstream) — Real-Time Threat Intelligence Pipeline
A distributed system that ingests security events, streams them through Kafka, detects attack patterns with sliding-window analysis, and displays live threat analytics on a cybersecurity dashboard.

[![CI](https://github.com/Aliromia21/threatstream/actions/workflows/ci.yml/badge.svg)](https://github.com/Aliromia21/threatstream/actions/workflows/ci.yml)


**7 containerized services** · Event API → Kafka → Consumer → PostgreSQL → Stats API → WebSocket → React Dashboard

- Kafka event streaming with 3 topics, partitioned by source IP for ordering
- Dual-write pattern: raw events + pre-aggregated counters for O(1) dashboard reads
- Brute force and port scan detection via in-memory sliding windows
- PostgreSQL LISTEN/NOTIFY bridges Consumer and Stats API — zero extra infrastructure
- Live dashboard with WebSocket updates, threat level indicator, and real-time charts
- Full testing pyramid: unit, integration, Docker build verification in CI

**Stack:** Node.js, TypeScript, Kafka, PostgreSQL, Express, React, Recharts, WebSocket, Docker, GitHub Actions

---

### [Monitoring Platform](https://github.com/Aliromia21/monitoring-platform) — Production-Style HTTP Monitoring SaaS
A monitoring engine for HTTP services with background workers, smart alerting, and a React dashboard. Inspired by Datadog and UptimeRobot.

 [![CI](https://github.com/Aliromia21/monitoring-platform/actions/workflows/api-ci.yml/badge.svg)](https://github.com/Aliromia21/monitoring-platform/actions/workflows/api-ci.yml)

- BullMQ producer/consumer with retry logic, dead letter queue, and horizontal scaling
- State machine alerting: DOWN → RECOVERY → SYSTEM_ERROR with consecutive failure thresholds
- Redis cache-aside pattern with automatic invalidation on write operations
- P95 response time via MongoDB aggregation pipeline
- 31 integration tests, CI/CD with GitHub Actions, code coverage via Codecov

**Stack:** Node.js, TypeScript, MongoDB, Redis, BullMQ, Express, React, Docker, GitHub Actions

---

## Tech Stack

**Core:** Node.js · TypeScript · Express · React  
**Streaming:** Apache Kafka · BullMQ · WebSocket  
**Databases:** PostgreSQL · MongoDB · Redis  
**DevOps:** Docker · Docker Compose · GitHub Actions · CI/CD  
**Testing:** Jest · Supertest · Integration & Unit Testing  
**Concepts:** Microservices · Event Streaming · CQRS · Pre-Aggregation · Sliding Window Detection · Graceful Shutdown

---

## Education

**M.Sc. Computer Science** — Technische Universität Braunschweig *(2025 – present)*  
**B.Sc. Computer Science** — Tishreen University *(2016 – 2022)*

---

## Languages

German (C1) · English (C1) · Arabic (Native)

---

## Connect

[LinkedIn](https://www.linkedin.com/in/aliromia/) · [GitHub](https://github.com/Aliromia21) · aliromiah13@gmail.com
