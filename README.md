# Вадим Евтеев

**Senior Java Engineer / Lead Backend Engineer**

evteewadim@gmail.com · [linkedin.com/in/evteevvadim](https://linkedin.com/in/evteevvadim) · [t.me/vadimevteev](https://t.me/vadimevteev) · Удалённо / Релокация

## О себе

Senior Java Engineer с 7+ годами опыта проектирования и разработки высоконагруженных распределённых систем (300+ RPS, 48ms P99 latency) в FinTech, AdTech и E-commerce. Глубокая экспертиза в Java, Spring Boot, Kafka и событийно-ориентированной микросервисной архитектуре. Проектировал отказоустойчивые системы от архитектуры до прода: Kafka exactly-once pipelines, zero-downtime миграции legacy-сервисов, reactive low-latency платформы. Опыт технического лидерства команд до 6 инженеров и принятия архитектурных решений в кросс-функциональных командах. Имею практический опыт разработки и вывода в продакшен backend-продуктов с интеграцией LLM и AI-сервисов. Разрабатывал production-решения с использованием LLM: структурирование данных, голосовые интерфейсы, AI-ассистенты, автоматизация бизнес-процессов. Ищу роль Senior Java / Lead Backend Engineer в продуктовой высоконагруженной команде.

## Опыт работы

### Freelance Senior Java Engineer | Independent Contractor | Авг 2025 — Настоящее время

- Разработал платёжного Telegram-бота для инфобизнеса: интеграция с платёжной системой LavaTop, автоматическое управление подписками в приватных каналах через Webhook и REST API.
- Разработал AI CRM для управления клиентскими контактами — голосовой ввод и транскрипция через Whisper, автоматическая структуризация профилей через GPT-4o, система follow-up предложений.
- Реализовал защиту от prompt injection на уровне системных промптов, добавил оценку уверенности ответов модели (confidence scoring) и опциональную проверку результата второй моделью.
- Спроектировал архитектуру AI-тренера по шахматам: реализовал гибридную схему, где для детерминированного анализа позиций используется движок Stockfish, а для генерации понятных пользователю объяснений — LLM. Настроил маршрутизацию запросов между моделями Claude и GPT через OpenRouter с учётом ограничений по token-budget.
- Спроектировал техническую архитектуру multi-agent AI платформы для стартапа — оркестрация продуктовых, дизайн- и технических ролей с автоматизированным тестированием.

**Стек:** Java, Python, PostgreSQL, Docker, GPT-4o, Claude API, OpenRouter, Whisper, Telegram Bot API, CI/CD

### Senior Software Engineer | LINEATE (AdTech) | Июн 2024 — Авг 2025

- Исполнял роль Acting Tech Lead (4–6 инженеров): sprint-церемонии, delivery ownership, координация команды, управление zero-downtime rollout через ArgoCD.
- Выступил архитектором и техническим лидером полной миграции legacy-сервиса с C# на реактивную Java-экосистему (Spring WebFlux): провёл аудит исходной архитектуры, выявил технические ограничения и спроектировал целевую архитектуру с расчётом на 10-кратный рост нагрузки — достигнуто 4-кратное улучшение throughput под нагрузочным тестированием, переход выполнен без остановки сервиса (Blue-Green deployment).
- Принял ключевые архитектурные решения: REST вместо gRPC на основе observability и стоимости миграции; централизованный Redis full-response cache вместо per-instance in-memory — существенно снизил нагрузку на БД.
- Заменил цепочки последовательных REST-запросов единым GraphQL API, упростив интеграцию для фронтенд-команды.
- Применил Virtual Threads для увеличения пропускной способности при параллельной обработке запросов.
- Проектировал стратегии безопасного развёртывания между регионами (Blue-Green, Rolling Update, Feature Flag) через ArgoCD — zero-downtime releases для high-load ad-систем.
- Разрабатывал и поддерживал reactive cloud-native low-latency сервисы: 300+ RPS на pod, 48ms P99, Spring WebFlux + Project Reactor.
- Устранил GC pressure и memory hotspots через профилирование; выполнил JVM tuning для стабильной работы под нагрузкой.

**Стек:** Java, Spring WebFlux, Project Reactor, Kafka, PostgreSQL, Redis, Docker, Kubernetes, ArgoCD, Prometheus, Grafana, CI/CD

### Software Engineer | EPAM Systems (GoDaddy) | Июл 2022 — Июн 2024

- Спроектировал и разработал распределённую микросервисную экосистему (6+ сервисов) под production-нагрузкой.
- Снизил P99 latency со ~150ms до ~60ms (-60%) по данным APM — через устранение N+1 ORM bottlenecks и оптимизацию data-fetching паттернов.
- Улучшил производительность критических SQL-запросов на 40% через переработку схем БД и целевую indexing strategy.
- Реализовал Kafka-based async communication для масштабируемой событийно-ориентированной архитектуры.
- Улучшил observability через ELK stack integration — сократил MTTD и ускорил реакцию на инциденты.
- Реализовал декомпозицию и миграцию критических модулей legacy C# сервиса на Java microservices, улучшив maintainability и performance.
- Реализовал SpEL-based фильтрацию данных и слой кеширования, существенно увеличив пропускную способность запросов.

**Стек:** Java 11–17, Spring Boot, Spring MVC, Spring Cloud, DynamoDB, AWS, Elasticsearch, Kafka, Docker, Kubernetes, OpenTelemetry, MapStruct, JWT, SonarQube, Jenkins, GitHub Actions

### Chief Software Engineer | SBERBANK (FinTech) | Сен 2021 — Июн 2022

- Проектировал распределённые процессы обработки этапов выпуска зарплатных карт, обеспечивая корректность и консистентность данных.
- Разработал Kafka pipelines со строгим порядком сообщений, exactly-once processing semantics и идемпотентными consumer handlers — гарантия отсутствия дублирования транзакций.
- Реализовал механизмы идемпотентности и retry-логику между сервисами.
- Разработал переиспользуемую audit-библиотеку на Spring AOP — внедрена во все сервисы команды (4+ сервиса), устранила дублирование audit-логики и обеспечила единый compliance trail.
- Менторил junior-инженеров по архитектурным решениям, паттернам распределённых систем и clean-code практикам.
- Интегрировал разнородные сервисы через REST и SOAP; разрабатывал REST API с управлением миграциями схем через Liquibase.

**Стек:** Java 8/11, Spring Boot, Spring Data, AOP, Hibernate, Liquibase, Apache Kafka, PostgreSQL, OpenShift, Docker, Maven, JUnit, Mockito, SonarQube, Jenkins

### Java Software Engineer | Reliability Technologies (FinTech / HealthTech) | Окт 2018 — Авг 2021

- Разрабатывал backend-сервисы и REST API для мобильных и web CRM-приложений корпоративных банковских клиентов (Банк Открытие) — API и модели данных оптимизированы под мобильные устройства: минимизация payload, быстрый client-server round-trip.
- Спроектировал микросервисную архитектуру и модели данных с нуля; реализовал RabbitMQ-based messaging между сервисами.
- Автоматизировал процессы развёртывания и контроля качества через настройку CI/CD pipelines (Jenkins, SonarQube); участвовал в code review и улучшении качества legacy систем.

**Стек:** Java 8, Spring Boot, Spring AOP, RabbitMQ, PostgreSQL, MySQL, Docker, Jenkins, Swagger, Git, SonarQube

## Навыки

- **Языки:** Java (8–21), Kotlin, Python, JavaScript, SQL
- **JVM и многопоточность:** JVM Internals, Многопоточность, GC Tuning, Lock-free Design
- **Фреймворки:** Spring Boot, Spring WebFlux, Spring MVC, Spring Data, Spring Security, Spring AOP, Hibernate, Liquibase
- **Базы данных:** PostgreSQL, MySQL, DynamoDB, Redis, Elasticsearch, Supabase
- **Очереди сообщений:** Apache Kafka (exactly-once, порядок, партиционирование), RabbitMQ
- **DevOps и облако:** Docker, Kubernetes, OpenShift, AWS, ArgoCD, CI/CD (Jenkins, GitHub Actions), Prometheus, Grafana
- **Ключевые паттерны:** Распределённые транзакции, Идемпотентность, Exactly-once Delivery, Failure Handling, CQRS, Event-Driven, High-Availability, Аудит и миграция legacy-систем
- **API и тестирование:** REST, gRPC, SOAP, GraphQL, OpenAPI/Swagger, Mobile Backend APIs, JUnit 5, Mockito, Load Testing
- **AI-интеграции:** Claude API, GPT-4o, OpenRouter, Whisper, AI Agent Workflows, Prompt Engineering, Контроль качества ответов LLM
- **AI-инструменты в разработке:** Claude Code, ChatGPT, Gemini

## Образование

**Белгородский государственный университет** — Магистр, Информационные системы и технологии, 2020
Институт инженерных и цифровых технологий

## Языки

Английский — C1 (Advanced)
