# Vadim Evteev

**Senior Java Backend Engineer**

evteewadim@gmail.com · [linkedin.com/in/evteevvadim](https://linkedin.com/in/evteevvadim) · [t.me/vadimevteev](https://t.me/vadimevteev)<br>
Remote B2B contracts · Open to relocation

## About

Senior Java Backend Engineer with 7+ years of experience building and modernizing distributed systems in FinTech, AdTech, and e-commerce. Core stack: Java 8–21, Spring Boot and WebFlux, Kafka, PostgreSQL, Redis, Kubernetes; focused on backend performance, reliability, and observability.

- Led a C#-to-Java service migration that raised throughput from 350 to 1,400 RPS in load tests and reached 300+ RPS per pod at 48 ms P99 in production.
- Cut P99 latency from 150 ms to 60 ms in a distributed system of 6+ services; built transactional Kafka processing with idempotent consumers and an outbox for bank card issuance flows.
- Periodically covered for the Team Lead of a 4–6 engineer team and mentored junior engineers.
- Since 2025, independently designing and shipping production client products with LLM integrations: RAG, queues, and idempotent webhook pipelines.

Open to remote Senior Java Backend Engineer roles, including B2B contracts.

## Work Experience

### Independent Software Engineer | Client Products and AI Automation | Aug 2025 — Present

- Architected and built **Business Honest**, a CRM and AI sales-enablement platform for a B2B business school: a Fastify/PostgreSQL core service with server-side authentication and RBAC, client and call histories, background jobs, and an auditable error log; a React portal and a Telegram Mini App where managers handle clients, contacts, and call history from their phones.
- Integrated Zoom: Server-to-Server OAuth, signed webhook verification, idempotent call synchronization with deduplication of repeated events, transcripts, and AI Companion summaries. Implemented AI call classification and on-demand generation of versioned, editable follow-up drafts and structured preparation briefs for the next sales call through OpenRouter, with Telegram delivery and Google Drive adapters.
- Implemented a Retrieval-Augmented Generation (RAG) pipeline over a versioned PostgreSQL knowledge base: deterministic SQL retrieval, Full-Text Search with Russian lexeme matching, tag-based scoring, and synonym/alias search. Added code-level source verification of generated claims (grounding guardrails), so facts about tariffs, cases, modules, and business mechanics reach the output only from verified records.
- Built and deployed a multilingual first-line AI bot for **Bali DJ School**'s Instagram Direct on Cloudflare Workers, TypeScript, Supabase, and OpenRouter: knowledge-base answers, seven-step lead qualification, objection handling, and Telegram handoff to a manager. Made it reliable with PGMQ queues, a durable outbox, per-lead concurrency control, bounded retries, and regression tests.
- Delivered **BuildTrack**, a role-based construction-management platform for the UAE market on Next.js/TypeScript/Supabase: dashboards for clients, contractors, managers, and admins covering tenders, contracts, budgets, work reports, payments, and notifications; integrated a Flask public showcase and admin, and set up a Dockerized two-service deployment.

**Stack:** TypeScript, Node.js, Python, Fastify, React, Next.js, Cloudflare Workers, Flask, PostgreSQL, Supabase, pg-boss, PGMQ, Docker, OpenRouter, Zoom API, Instagram Graph API, Telegram Bot API and Mini Apps, Google Drive API, CI/CD

### Senior Software Engineer | LINEATE (AdTech) | Jun 2024 — Aug 2025

- Periodically covered for the Team Lead of a 4–6 engineer team, taking ownership of selected responsibilities depending on workload, including technical coordination, architectural decisions, and rollout planning.
- Led the migration of a legacy C# landing service to Java and Spring WebFlux. The target architecture was designed for an expected 10x increase in both request rate and JSON payload volume; load tests confirmed a 4x throughput increase from 350 to 1,400 RPS.
- Performed the migration and operated the service across two regions and eight pods; production performance reached 300+ RPS per pod at 48 ms P99. Designed Blue-Green, Rolling Update, and Feature Flag deployment strategies with ArgoCD.
- Made the architectural decision to use REST instead of gRPC after analyzing migration cost and observability requirements; introduced centralized Redis full-response caching to reduce database load.
- Replaced chains of sequential REST requests with a single GraphQL endpoint, reducing client round trips and simplifying frontend integration. Used Virtual Threads separately for a blocking workload to increase concurrency.
- Eliminated GC pressure and memory hotspots through profiling and JVM tuning.

**Stack:** Java, Spring WebFlux, Project Reactor, Kafka, PostgreSQL, Redis, Docker, Kubernetes, ArgoCD, Prometheus, Grafana, CI/CD

### Software Engineer | EPAM Systems — GoDaddy | Jul 2022 — Jun 2024

- Designed and developed a distributed ecosystem of 6+ Java services under production load.
- Reduced P99 latency from approximately 150 ms to 60 ms (60%) by eliminating N+1 ORM bottlenecks and optimizing data-fetching patterns.
- Improved critical SQL query performance by 40% through schema changes and targeted indexing.
- Introduced Kafka-based asynchronous communication and improved observability with ELK and OpenTelemetry, reducing detection and incident investigation time.
- Decomposed and migrated critical modules from a legacy C# service to maintainable Java microservices.

**Stack:** Java 11–17, Spring Boot, Spring MVC, Spring Cloud, DynamoDB, AWS, Elasticsearch, Kafka, Docker, Kubernetes, OpenTelemetry, JWT, SonarQube, Jenkins, GitHub Actions

### Chief Software Engineer | SBERBANK (FinTech) | Sep 2021 — Jun 2022

- Designed distributed workflows for payroll card issuance, ensuring data consistency across processing stages.
- Implemented Kafka transactions with transactional producers and offset commits, together with idempotent consumers and outbox handling for database side effects; preserved strict ordering and prevented duplicate processing in card-issuance workflows.
- Built a reusable audit library with Spring AOP, adopted across 4+ team services to provide a unified compliance trail and remove duplicated audit logic.
- Integrated heterogeneous services through REST and SOAP and managed database schema migrations with Liquibase.
- Mentored junior engineers on distributed-systems patterns, architectural decisions, and clean-code practices.

**Stack:** Java 8/11, Spring Boot, Spring Data, AOP, Hibernate, Liquibase, Apache Kafka, PostgreSQL, OpenShift, Docker, Maven, JUnit, Mockito, SonarQube, Jenkins

### Java Software Engineer | Reliability Technologies (FinTech / HealthTech) | Oct 2018 — Aug 2021

- Developed backend services and REST APIs for mobile and web CRM applications used by corporate banking clients, including Bank Otkritie.
- Designed microservice architecture and data models from scratch and implemented RabbitMQ-based messaging between services.
- Automated deployment and quality controls with Jenkins and SonarQube and contributed to code reviews and legacy-system improvements.

**Stack:** Java 8, Spring Boot, Spring AOP, RabbitMQ, PostgreSQL, MySQL, Docker, Jenkins, Swagger, Git, SonarQube

## Skills

- **Java:** Java 8–21, concurrency, Virtual Threads, JVM profiling, GC tuning
- **Frameworks:** Spring Boot, Spring WebFlux, Spring MVC, Spring Data, Spring Security, Spring AOP, Hibernate, Liquibase
- **Data and Messaging:** PostgreSQL, MySQL, DynamoDB, Redis, Elasticsearch, Apache Kafka, RabbitMQ
- **Cloud and Delivery:** AWS, Docker, Kubernetes, OpenShift, ArgoCD, Jenkins, GitHub Actions, Prometheus, Grafana, OpenTelemetry
- **Architecture and APIs:** Distributed systems, event-driven architecture, idempotency, failure handling, REST, SOAP, GraphQL, gRPC, OpenAPI
- **Testing:** JUnit 5, Mockito, integration and load testing, SonarQube
- **Additional Product Stack:** TypeScript, Node.js, Fastify, React, Next.js, Cloudflare Workers, Supabase, Python, Flask, Telegram Mini Apps
- **AI and Product Integrations:** Retrieval-Augmented Generation (RAG), prompt engineering, LLM guardrails, structured LLM outputs, OpenRouter, OpenAI API, Claude API, Zoom API, Instagram Graph API, Telegram Bot API, Google Drive API

## Education

**Belgorod State University** — Master's Degree in Information Systems and Technologies, 2020<br>
Institute of Engineering and Digital Technologies

## Languages

English — Advanced (C1)
