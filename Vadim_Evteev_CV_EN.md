# Vadim Evteev

**Senior Java Engineer / Lead Backend Engineer**

evteewadim@gmail.com · [linkedin.com/in/evteevvadim](https://linkedin.com/in/evteevvadim) · [t.me/vadimevteev](https://t.me/vadimevteev) · Remote / Relocation

## About

Senior Java Engineer with 7+ years of experience designing and building high-scale distributed systems (300+ RPS, 48ms P99 latency) in FinTech, AdTech, and E-commerce. Deep expertise in Java, Spring Boot, Kafka, and event-driven microservice architecture. Designed fault-tolerant systems from architecture to production: Kafka exactly-once pipelines, zero-downtime legacy migrations, reactive low-latency platforms. Proven track record of legacy system takeover — auditing architecture, identifying technical debt, and driving improvement plans. AI-assisted development practitioner: builds and ships AI-integrated backend products. Experience leading engineering teams of up to 6 engineers and making architectural decisions in cross-functional teams. Seeking Senior Java or Lead Backend Engineering opportunities in high-scale product companies.

## Work Experience

### Senior Java Engineer | Freelance / Independent Contractor | Aug 2025 — Present

- Built an AI CRM for contact management: voice input transcribed via Whisper, automated contact profile enrichment via GPT-4o, follow-up recommendation generation.
- Implemented prompt-injection protection (system-prompt priority) and hallucination control — engine output as ground truth, confidence scoring, optional second-model verification.
- Designed an educational chess platform with AI trainer: Stockfish wrapper for ground-truth analysis + LLM move explanations; intelligent model routing between Claude and GPT via OpenRouter with token-budget-based model downgrade.
- Built a payment Telegram bot for EdTech businesses: integrated with the LavaTop payment system, automated subscription management in private channels via Webhook and REST API.
- Designed the technical architecture of a multi-agent AI platform for a startup — orchestration of product, design, and engineering roles with automated testing.

**Stack:** Java, Python, PostgreSQL, Docker, GPT-4o, Claude API, OpenRouter, Whisper, Telegram Bot API, CI/CD

### Senior Software Engineer | LINEATE (AdTech) | Jun 2024 — Aug 2025

- Took over a legacy C# service as technical owner: audited the architecture and code, identified critical technical debt (N+1 query problems, missing distributed caching), and drove the prioritized improvement plan.
- Led complete architectural migration of the legacy C# landing service to a reactive Java ecosystem (Spring WebFlux) targeting 10x load growth — achieved 4x throughput improvement under load testing, zero downtime via Blue-Green deployment.
- Served as Acting Technical Lead for a team of 4–6 engineers: technical leadership, delivery ownership, team coordination, zero-downtime rollout management via ArgoCD.
- Made key architectural decisions: REST over gRPC based on observability and migration cost; centralized Redis full-response cache over per-instance in-memory — significantly reduced database load.
- Resolved N+1-style chained-request problems by introducing GraphQL; increased parallel-processing throughput with Virtual Threads.
- Designed safe deployment strategies across regions (Blue-Green, Rolling Update, Feature Flag) via ArgoCD — zero-downtime releases for high-scale ad systems.
- Developed and maintained reactive cloud-native low-latency services: 300+ RPS per pod, 48ms P99, Spring WebFlux + Project Reactor.
- Eliminated GC pressure and memory hotspots through profiling; performed JVM tuning for stable operation under load.

**Stack:** Java, Spring WebFlux, Project Reactor, Kafka, PostgreSQL, Redis, Docker, Kubernetes, ArgoCD, Prometheus, Grafana, CI/CD

### Software Engineer | EPAM Systems (GoDaddy) | Jul 2022 — Jun 2024

- Designed and built a distributed microservice ecosystem (6+ services) under production load.
- Reduced P99 latency from ~150ms to ~60ms (-60%) per APM data — by eliminating N+1 ORM bottlenecks and optimizing data-fetching patterns.
- Improved critical SQL query performance by 40% through database schema redesign and targeted indexing strategy.
- Implemented Kafka-based async communication for scalable event-driven architecture.
- Implemented SpEL-based data filtering and a caching layer, significantly increasing request throughput.
- Improved observability via ELK stack integration — reduced MTTD and accelerated incident response.
- Decomposed and migrated critical modules of a legacy C# service to Java microservices, improving maintainability and performance.

**Stack:** Java 11–17, Spring Boot, Spring MVC, Spring Cloud, DynamoDB, AWS, Elasticsearch, Kafka, Docker, Kubernetes, OpenTelemetry, MapStruct, JWT, SonarQube, Jenkins, GitHub Actions

### Chief Software Engineer | SBERBANK (FinTech) | Sep 2021 — Jun 2022

- Designed distributed processes for payroll card issuance stages, ensuring data correctness and consistency.
- Built Kafka pipelines with strict message ordering, exactly-once processing semantics, and idempotent consumer handlers — preventing duplicate transaction processing.
- Implemented idempotency mechanisms and retry logic between services.
- Developed a reusable audit library on Spring AOP — deployed across all team services (4+), eliminating audit logic duplication and providing a unified compliance trail.
- Mentored junior engineers on architectural decisions, distributed systems patterns, and clean-code practices.
- Integrated heterogeneous services via REST and SOAP; developed REST APIs with schema migration management via Liquibase.

**Stack:** Java 8/11, Spring Boot, Spring Data, AOP, Hibernate, Liquibase, Apache Kafka, PostgreSQL, OpenShift, Docker, Maven, JUnit, Mockito, SonarQube, Jenkins

### Java Software Engineer | Reliability Technologies (FinTech / HealthTech) | Oct 2018 — Aug 2021

- Developed backend services and REST APIs for mobile and web CRM applications for corporate banking clients (Bank Otkritie) — APIs and data models optimized for mobile: minimized payload, fast client-server round-trip.
- Designed microservice architecture and data models from scratch; implemented RabbitMQ-based messaging between services.
- Automated deployment and quality assurance processes by configuring CI/CD pipelines (Jenkins, SonarQube); participated in code reviews and legacy system quality improvement.

**Stack:** Java 8, Spring Boot, Spring AOP, RabbitMQ, PostgreSQL, MySQL, Docker, Jenkins, Swagger, Git, SonarQube

## Skills

- **Languages:** Java (8–21), Kotlin, Python, JavaScript, SQL
- **JVM & Concurrency:** JVM Internals, Java Concurrency, GC Tuning, Lock-free Design
- **Frameworks:** Spring Boot, Spring WebFlux, Spring MVC, Spring Data, Spring Security, Spring AOP, Hibernate, Liquibase
- **Databases:** PostgreSQL, MySQL, DynamoDB, Redis, Elasticsearch, Supabase
- **Messaging:** Apache Kafka (exactly-once, ordering, partitioning), RabbitMQ
- **DevOps & Cloud:** Docker, Kubernetes, OpenShift, AWS, ArgoCD, CI/CD (Jenkins, GitHub Actions), Prometheus, Grafana
- **Key Patterns:** Distributed Transactions, Idempotency, Exactly-once Delivery, Failure Handling, CQRS, Event-Driven, High-Availability, Legacy Takeover & Migration
- **API & Testing:** REST, gRPC, SOAP, GraphQL, OpenAPI/Swagger, Mobile Backend APIs, JUnit 5, Mockito, Load Testing
- **AI Integrations:** Claude API, GPT-4o, OpenRouter, Whisper, AI Agent Workflows, Prompt Engineering, Hallucination Control
- **AI-Assisted Dev:** Claude Code, ChatGPT, Gemini — actively used in engineering workflow

## Education

**Belgorod State University** — Master's Degree, Information Systems and Technologies, 2020
Institute of Engineering and Digital Technologies

## Languages

English — Advanced (C1)
