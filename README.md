# 🌐 jackydev95 | Senior Java Software Engineer

<p align="center">
  <a href="https://t.me/jackydev95">
    <img src="https://img.shields.io/badge/Telegram-Join%20Us-26A69A?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram">
  </a>
  <a href="https://jackydev95.online/">
    <img src="https://img.shields.io/badge/Website-Visit%20Site-4CAF50?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Website">
  </a>
  <a href="https://github.com/jackydev95">
    <img src="https://img.shields.io/github/followers/jackydev95?label=Followers&style=for-the-badge&logo=github&color=2196F3&logoColor=white" alt="Followers">
  </a>
  <a href="https://github.com/jackydev95?tab=following">
    <img src="https://img.shields.io/badge/Following-30.2K-FF9800?style=for-the-badge&logo=github&logoColor=white" alt="Following">
  </a>
</p>

---

## 🌟 About Me & Engineering Philosophy

I am a **Senior Java Developer** specializing in building highly scalable, resilient, and enterprise-grade backend systems. I design and implement backend architectures using **Domain-Driven Design (DDD)** and **Hexagonal Architecture (Ports and Adapters)**, ensuring that the domain logic remains pure and decoupled from infrastructure and frameworks.

### 🛡️ Core Pillars

- ⚡ **Domain-Driven Design**: Modeling rich domains, value objects, and aggregate roots to accurately reflect business rules.
- 📦 **Hexagonal Architecture**: Strict separation of concerns (Presentation → Application → Domain ← Infrastructure) with clear dependency inversion.
- 🧩 **Use Case & Port Patterns**: Encapsulating transaction orchestration and validating input boundaries cleanly.
- 🔗 **Robust Integration**: Designing high-performance API portals, message queues, and caching systems.

---

## 🧩 Architectural Patterns & Implementation Standards

I adhere to strict software design patterns to ensure maximum maintainability, testability, and decoupling:

| Architectural Pattern | Status | Description | Standard Implementation |
| :--- | :---: | :--- | :---: |
| **Domain Isolation** | 🟢 Active | Domain layer has zero dependencies on frameworks, databases, or external services. | Pure Java |
| **Repository Pattern** | 🟢 Active | Interface defined in `domain/repository/`, JPA implementations in `infrastructure/persistence/`. | Spring Data JPA / Hibernate |
| **Use Case Pattern** | 🟢 Active | Dedicated input command validation, core business logic orchestration, and output results. | Port In / UseCaseImpl |
| **Port Out Pattern** | 🟢 Active | Outward ports defined in Application layer *only* for external integrations (SMS, Mail, Payments). | Web Clients / SDK Adapters |
| **Hexagonal Routing** | 🟢 Active | Controllers map REST/GraphQL requests to Command DTOs and return Responses mapped from Result DTOs. | Spring MVC / GraphQL |
| **Test-Driven Design** | 🟢 Active | 100% coverage on domain logic and application services using mocks and fixtures. | JUnit 5 / Mockito |

---

## 🛠️ Technology & Infrastructure Stack

### Languages & Frameworks

<p align="left">
  <img alt="Java" src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
  <img alt="Spring Boot" src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white" />
  <img alt="Spring Security" src="https://img.shields.io/badge/Spring_Security-6DB33F?style=for-the-badge&logo=spring&logoColor=white" />
  <img alt="Hibernate" src="https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=hibernate&logoColor=white" />
  <img alt="Gradle" src="https://img.shields.io/badge/Gradle-02303A?style=for-the-badge&logo=gradle&logoColor=white" />
  <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white" />
  <img alt="React" src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" />
</p>

### Infrastructure, Caching & Cloud

<p align="left">
  <img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img alt="Redis" src="https://img.shields.io/badge/Redis-CC0000?style=for-the-badge&logo=redis&logoColor=white" />
  <img alt="Docker" src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img alt="AWS" src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white" />
  <img alt="Kubernetes" src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" />
  <img alt="Kafka" src="https://img.shields.io/badge/Kafka-231F20?style=for-the-badge&logo=apache-kafka&logoColor=white" />
  <img alt="Traefik" src="https://img.shields.io/badge/Traefik-24A1C1?style=for-the-badge&logo=traefik&logoColor=white" />
</p>

---

## ⚙️ Architecture & Design Patterns Deep-Dive

<details>
<summary><b>🔥 Spring Boot Domain-Driven Design (DDD)</b></summary>

- **Clean Layer Separation** – Strict flow: `Presentation` (REST Controllers) → `Application` (Use Cases) → `Domain` (Core Models) ← `Infrastructure` (JPA/Adapters).
- **Dependency Inversion** – Domain layer has zero dependencies on databases or frameworks. Interface adapters handle concrete data operations.
- **Transactional Consistency** – Application layer manages transactional boundaries `@Transactional` coordinating entities and domain repositories.
</details>

<details>
<summary><b>💾 Persistence, Caching & Event Sourcing</b></summary>

- **JPA & Hibernate Mapping** – Clear separation of JPA entities (`infrastructure/persistence/entity/`) and pure domain models (`domain/model/`).
- **Distributed Caching** – Dual-layer cache strategy using localized Spring cache and centralized `Redis` cluster configuration.
- **Relational & NoSQL Systems** – High-performance transactional persistence with `PostgreSQL` and single-table DynamoDB layouts.
- **Event-Driven Messaging** – Real-time event propagation via `Apache Kafka` topic publishers and async listener ports.
</details>

<details>
<summary><b>🛡️ Security, Testing & DevOps Orchestration</b></summary>

- **OAuth2 & JWT Security** – Role-Based Access Control (RBAC) and security filters configured via Spring Security.
- **Rigorous Test Suites** – High-coverage JUnit 5 unit testing with Mockito mocks, and Spring Boot integration tests utilizing Testcontainers.
- **Infrastructure as Code (IaC)** – Automated cloud deployment via AWS ECS, Kubernetes configurations, and Terraform modules.
- **Telemetry & Monitoring** – Live application metrics using Prometheus, Micrometer, and Grafana telemetry dashboards.
</details>

---

## 🤖 AI-Native Engineering

I leverage cutting-edge autonomous engineering models to build, maintain, and optimize software systems.

<details>
<summary><b>🤖 Google Antigravity & Agentic AI</b></summary>

- [**Antigravity by Google**](https://antigravity.google) – Next-generation agentic AI framework for high-autonomy coding and systems engineering.
- [**Antigravity Skills Codelab**](https://codelabs.developers.google.com/getting-started-with-antigravity-skills) – Interactive tutorial on configuring customized tools and skill pipelines for coding agents.
- [**Stitch by Google**](https://stitch.withgoogle.com/) – Experimental collaborative AI playground for rich context mapping.
</details>

<details>
<summary><b>💻 Coding Assistants & Playgrounds</b></summary>

- [**Cursor IDE**](https://www.cursor.com/) – State-of-the-art AI-first code editor designed for rapid prototyping.
- [**Claude AI**](https://claude.ai/new) – Advanced logic reasoning and context modeling helper.
- [**ChatGPT**](https://openai.com/chatgpt/) – Broad multitasking and creative prompt modeling assistant.
- [**Replit AI**](https://replit.com) – Cloud-hosted IDE featuring visual sandbox environments.
</details>

---

## 🔗 Developer Resources & Reference Guides

<details>
<summary><b>☕ Java & Spring Framework Reference</b></summary>

- [**Spring Boot Docs**](https://spring.io/projects/spring-boot) – Official Spring Boot documentation and reference guides.
- [**Baeldung Tutorials**](https://www.baeldung.com/) – Excellent Java and Spring framework tutorials.
- [**Refactoring.Guru**](https://refactoring.guru/) – Visual guide to software design patterns and refactoring techniques.
- [**Architecture Patterns Guide**](https://github.com/iluwatar/java-design-patterns) – Standard Java design patterns implementation library.
</details>

<details>
<summary><b>🌐 Cloud Integrations & Networks</b></summary>

- [**AWS SDK for Java**](https://aws.amazon.com/sdk-for-java/) – Developer resources for AWS integration.
- [**Docker Hub Portal**](https://hub.docker.com/) – Custom image orchestration and container publishing.
- [**Confluent Cloud**](https://confluent.cloud) – Apache Kafka cloud instances for message distribution.
- [**Cloudflare Portal**](https://dash.cloudflare.com) – Secure CDNs, DDoS protection, and SSL gateway management.
</details>

<details>
<summary><b>📚 Documentation & Standards</b></summary>

- [**Conventional Commits Standard**](https://conventionalcommits.org) – Specifications for structural git commits.
- [**Twelve-Factor App Methodology**](https://12factor.net/) – Best practices for building modern, cloud-native applications.
- [**HackTricks Handbook**](https://book.hacktricks.xyz) – Cyber security checklists and penetration testing methodologies.
</details>
