# Vadim Evteev

**Senior Java Backend Engineer**

evteewadim@gmail.com · [linkedin.com/in/evteevvadim](https://linkedin.com/in/evteevvadim) · [t.me/vadimevteev](https://t.me/vadimevteev)<br>
Remote B2B contracts · Available across UTC+4 to UTC+8 · Open to relocation

## About

Senior Java Backend Engineer with 7+ years of experience building and modernizing distributed systems in FinTech and AdTech. Led a C#-to-Java service migration that increased throughput from 350 to 1,400 RPS in load tests. Periodically covered selected Team Lead responsibilities based on team workload. Hands-on with Java, Spring Boot, Kafka, PostgreSQL, Redis, Kubernetes, performance optimization, and observability. Since 2025, I have also built backend prototypes with LLM integrations, including a Java backend for an AI-assisted contact CRM. Open to remote Senior Java Backend roles, including B2B contracts.

## Work Experience

### Independent Backend Engineer | Client and Product Prototypes | Aug 2025 — Present

- Built a Java backend prototype for a contact-management CRM, integrating Whisper voice transcription and GPT-4o-based extraction of structured contact data.
- Developed a client prototype for an online-education subscription service, integrating LavaTop webhooks and REST API with a Telegram bot to automate payment-based access to private channels.
- Built a chess-training prototype combining deterministic Stockfish analysis with LLM-generated explanations and model routing through OpenRouter.
- Designed the prototype architecture of a multi-agent startup platform, covering the orchestration of product, design, and engineering roles and automated testing workflows.

**Stack:** Java, Python, PostgreSQL, Docker, GPT-4o, Claude API, OpenRouter, Whisper, Telegram Bot API, CI/CD

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
- **AI Integrations:** Python, GPT-4o, Claude API, OpenRouter, Whisper, structured LLM outputs, model routing

## Education

**Belgorod State University** — Master's Degree in Information Systems and Technologies, 2020<br>
Institute of Engineering and Digital Technologies

## Languages

English — Advanced (C1)
