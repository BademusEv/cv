# Вадим Евтеев

**Senior Java Backend Engineer**

evteewadim@gmail.com · [linkedin.com/in/evteevvadim](https://linkedin.com/in/evteevvadim) · [t.me/vadimevteev](https://t.me/vadimevteev)<br>
Удалённые B2B-контракты · Готов к релокации

## О себе

Senior Java Backend Engineer с 7+ годами опыта разработки и модернизации распределённых систем в FinTech, AdTech и e-commerce. Основной стек: Java 8–21, Spring Boot и WebFlux, Kafka, PostgreSQL, Redis, Kubernetes; фокус — производительность, надёжность и наблюдаемость backend-систем.

- Руководил миграцией сервиса с C# на Java: пропускная способность в нагрузочных тестах выросла с 350 до 1 400 RPS, в production — 300+ RPS на pod при P99 48 мс.
- Снизил P99 latency со 150 до 60 мс в распределённой системе из 6+ сервисов; строил транзакционную обработку на Kafka с идемпотентными consumers и outbox в процессах выпуска банковских карт.
- Периодически замещал тимлида команды из 4–6 инженеров, менторил junior-разработчиков.
- С 2025 года самостоятельно проектирую и довожу до production клиентские продукты с LLM-интеграциями: RAG, очереди, идемпотентные webhook-пайплайны.

Рассматриваю удалённые позиции Senior Java Backend Engineer, в том числе по B2B-контракту.

## Опыт работы

### Независимый разработчик ПО | Клиентские продукты и AI-автоматизация | Авг 2025 — настоящее время

- Спроектировал и разработал **Business Honest** — CRM и AI-платформу поддержки B2B-продаж для бизнес-школы: core-сервис на Fastify/PostgreSQL с серверной аутентификацией и RBAC, историей клиентов и созвонов, фоновыми задачами и журналом ошибок; React-портал и Telegram Mini App, в котором менеджеры ведут клиентов, контакты и историю звонков с телефона.
- Интегрировал Zoom: Server-to-Server OAuth, проверка подписей webhook-событий, идемпотентная синхронизация звонков с дедупликацией повторных событий, транскрипции и сводки AI Companion. Реализовал AI-классификацию созвонов и генерацию по запросу версионируемых, редактируемых черновиков follow-up и структурированной подготовки менеджера к следующему созвону через OpenRouter, с доставкой в Telegram и адаптерами Google Drive.
- Реализовал RAG-пайплайн (Retrieval-Augmented Generation) поверх версионируемой базы знаний в PostgreSQL: детерминированный SQL retrieval, Full-Text Search с обработкой русских лексем, скоринг по тегам и поиск по синонимам/алиасам. Добавил программную проверку утверждений по источникам (grounding guardrails): факты о тарифах, кейсах, модулях и бизнес-механиках попадают в результат только из проверенных записей.
- Разработал и развернул многоязычного AI-бота первой линии для Instagram Direct школы **Bali DJ School** на Cloudflare Workers, TypeScript, Supabase и OpenRouter: ответы по базе знаний, семишаговая квалификация лидов, работа с возражениями и передача менеджеру в Telegram. Надёжность обеспечил PGMQ-очередями, outbox, контролем конкурентной обработки одного лида, ограниченными повторами и регрессионными тестами.
- Разработал **BuildTrack** — ролевую платформу управления строительными проектами для рынка ОАЭ на Next.js/TypeScript/Supabase: кабинеты заказчиков, подрядчиков, менеджеров и администраторов с тендерами, договорами, бюджетами, отчётами о работах, платежами и уведомлениями; интегрировал витрину и админку на Flask, настроил Docker-деплой двух сервисов.

**Стек:** TypeScript, Node.js, Python, Fastify, React, Next.js, Cloudflare Workers, Flask, PostgreSQL, Supabase, pg-boss, PGMQ, Docker, OpenRouter, Zoom API, Instagram Graph API, Telegram Bot API и Mini Apps, Google Drive API, CI/CD

### Senior Software Engineer | LINEATE (AdTech) | Июн 2024 — авг 2025

- Периодически замещал тимлида команды из 4–6 инженеров и в зависимости от загрузки брал на себя часть его обязанностей: координацию технической работы, архитектурные решения и планирование развёртываний.
- Руководил миграцией legacy-сервиса с C# на Java и Spring WebFlux. Целевая архитектура проектировалась под ожидаемый десятикратный рост количества запросов и объёма JSON-данных; нагрузочные тесты подтвердили четырёхкратный рост пропускной способности — с 350 до 1 400 RPS.
- Выполнял миграцию и обеспечивал эксплуатацию сервиса в двух регионах на восьми pod; производительность в production достигала 300+ RPS на pod при P99 48 мс. Спроектировал стратегии развёртывания Blue-Green, Rolling Update и Feature Flag в ArgoCD.
- Принял архитектурное решение использовать REST вместо gRPC после анализа стоимости миграции и требований к наблюдаемости; внедрил централизованное кеширование полных ответов в Redis, снизив нагрузку на базу данных.
- Заменил цепочки последовательных REST-запросов единым GraphQL endpoint, сократив количество клиент-серверных обменов и упростив интеграцию с frontend. В отдельной блокирующей нагрузке применил Virtual Threads для увеличения параллелизма.
- Устранил повышенную нагрузку на GC и узкие места в памяти с помощью профилирования и настройки JVM.

**Стек:** Java, Spring WebFlux, Project Reactor, Kafka, PostgreSQL, Redis, Docker, Kubernetes, ArgoCD, Prometheus, Grafana, CI/CD

### Software Engineer | EPAM Systems — GoDaddy | Июл 2022 — июн 2024

- Спроектировал и разработал распределённую систему из 6+ Java-сервисов под production-нагрузкой.
- Снизил P99 latency примерно со 150 до 60 мс (на 60%), устранив N+1-проблемы ORM и оптимизировав получение данных.
- Ускорил критические SQL-запросы на 40% за счёт изменений схемы базы данных и целевой настройки индексов.
- Внедрил асинхронное взаимодействие через Kafka и улучшил наблюдаемость с помощью ELK и OpenTelemetry, сократив время обнаружения и расследования инцидентов.
- Декомпозировал и перенёс критические модули legacy-сервиса с C# на Java-микросервисы.

**Стек:** Java 11–17, Spring Boot, Spring MVC, Spring Cloud, DynamoDB, AWS, Elasticsearch, Kafka, Docker, Kubernetes, OpenTelemetry, JWT, SonarQube, Jenkins, GitHub Actions

### Chief Software Engineer | СБЕРБАНК (FinTech) | Сен 2021 — июн 2022

- Проектировал распределённые процессы выпуска зарплатных карт, обеспечивая консистентность данных между этапами обработки.
- Реализовал Kafka-транзакции с транзакционными producers и фиксацией offsets, идемпотентные consumers и outbox для побочных эффектов в базе данных; обеспечил строгий порядок сообщений и защиту от повторной обработки в процессах выпуска карт.
- Разработал переиспользуемую библиотеку аудита на Spring AOP, внедрённую в 4+ сервисах команды: она обеспечила единый журнал для compliance-задач и устранила дублирование audit-логики.
- Интегрировал разнородные сервисы через REST и SOAP и управлял миграциями схем базы данных с помощью Liquibase.
- Менторил junior-инженеров по паттернам распределённых систем, архитектурным решениям и практикам чистого кода.

**Стек:** Java 8/11, Spring Boot, Spring Data, AOP, Hibernate, Liquibase, Apache Kafka, PostgreSQL, OpenShift, Docker, Maven, JUnit, Mockito, SonarQube, Jenkins

### Java Software Engineer | Reliability Technologies (FinTech / HealthTech) | Окт 2018 — авг 2021

- Разрабатывал backend-сервисы и REST API для мобильных и web CRM-приложений корпоративных банковских клиентов, включая Банк Открытие.
- Спроектировал микросервисную архитектуру и модели данных с нуля; реализовал обмен сообщениями через RabbitMQ.
- Автоматизировал развёртывание и контроль качества с помощью Jenkins и SonarQube, участвовал в code review и улучшении legacy-систем.

**Стек:** Java 8, Spring Boot, Spring AOP, RabbitMQ, PostgreSQL, MySQL, Docker, Jenkins, Swagger, Git, SonarQube

## Навыки

- **Java:** Java 8–21, многопоточность, Virtual Threads, профилирование JVM, настройка GC
- **Фреймворки:** Spring Boot, Spring WebFlux, Spring MVC, Spring Data, Spring Security, Spring AOP, Hibernate, Liquibase
- **Данные и очереди:** PostgreSQL, MySQL, DynamoDB, Redis, Elasticsearch, Apache Kafka, RabbitMQ
- **Облака и поставка:** AWS, Docker, Kubernetes, OpenShift, ArgoCD, Jenkins, GitHub Actions, Prometheus, Grafana, OpenTelemetry
- **Архитектура и API:** распределённые системы, событийная архитектура, идемпотентность, обработка отказов, REST, SOAP, GraphQL, gRPC, OpenAPI
- **Тестирование:** JUnit 5, Mockito, интеграционное и нагрузочное тестирование, SonarQube
- **Дополнительный продуктовый стек:** TypeScript, Node.js, Fastify, React, Next.js, Cloudflare Workers, Supabase, Python, Flask, Telegram Mini Apps
- **AI и продуктовые интеграции:** Retrieval-Augmented Generation (RAG), prompt engineering, LLM guardrails, структурированный вывод LLM, OpenRouter, OpenAI API, Claude API, Zoom API, Instagram Graph API, Telegram Bot API, Google Drive API

## Образование

**Белгородский государственный университет** — магистр, информационные системы и технологии, 2020<br>
Институт инженерных и цифровых технологий

## Языки

Английский — C1 (Advanced)
