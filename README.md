# Hi there 👋

I'm a **Software Developer** focused on building full-stack applications, backend systems, and production-ready software.

I enjoy turning ideas into real products, working across the entire development lifecycle — from designing and developing applications to testing, deployment, and infrastructure.

> 🔒 **Proprietary Software & Production Safety:** To protect production infrastructure from unauthorized access, automated scanning, and malicious requests, all direct URLs, endpoints, and credentials for my live SaaS applications are kept strictly private. Below is the architectural and engineering breakdown of the production-ready systems I design, build, and maintain.

---

## 🚀 Live SaaS Products & Applications

### 🛠️ Artisan Platform (Event-Driven Multi-Tenant ERP)
A multi-service **Enterprise Resource Planning (ERP) monorepo** designed for small business management, inventory orchestration, and financial tracking. The platform operates securely through a React-based administration dashboard and a core Go API, leveraging asynchronous messaging for business logic decoupled executions.

* **🟢 Status:** Fully deployed and active in production.
* **🔧 Operations:** Multi-service system composed of a core domain API, an administration dashboard, and messaging queues.

![Artisan Platform Interface Overview](https://github.com/marvini86/marvini86/blob/main/images/artisan.png?raw=true)

#### 🛠️ Core Architecture & Tech Stack
* **Backend API:** Go (Gin Framework, GORM) • JWT & OAuth 2.0 • PostgreSQL • OpenAPI/Swagger (Orval Client Generator) • **Azure Service Bus**
* **Frontend Apps:** React • TanStack Query • Tailwind CSS • React Router
* **Cloud & Infrastructure:** Oracle Cloud VPS (Backend hosting) • Azure Static Web Apps (Frontend) • Azure API Management (API Gateway) • Azure Blob Storage (Media/Asset Delivery) • Docker
* **CI/CD & DevOps:** GitHub Actions Automated Pipelines • Git

#### 🏗️ System Components & Engineering Highlights
* **Administration Dashboard:** A React interface used to manage multi-tenant domain operations, metrics tracking, and product distribution.
* **Core API Operations:** A high-performance Go API instance responsible for handling client requests, payload mapping, dynamic multi-tenant verification, and request logging.
* **Event-Driven Inventory Automation:** Integrated **Azure Service Bus** to handle asynchronous inventory lifecycle events. Whenever a sale is finalized, cancelled, or updated, the core API publishes transaction events to a message queue. Dedicated consumer routines process these events asynchronously to safely deduct or revert physical stock, ensuring ledger resilience and preventing database race conditions during concurrent usage.
* **Production-Grade Infrastructure & QA:** Automated CI/CD pipeline via GitHub Actions that builds Docker containers and triggers production updates on push. Secured and rate-limited public endpoints using Azure API Management, and covered with automated tests.

---

### 📺 Panel Management App (OOH Media Platform)
A full-stack **Out-of-Home (OOH) media management platform** designed to orchestrate and stream digital advertising content across distributed physical panels. 

I designed and engineered this entire platform end-to-end—building the high-performance Go API, the admin control center, and the edge media player that runs on connected physical hardware.

* **🟢 Status:** Fully deployed and active in production.
* **🔧 Operations:** Multi-service system composed of a central API, an admin portal, and dedicated hardware media player clients.

![Panel Management App Interface Overview](https://github.com/marvini86/marvini86/blob/main/images/panel.png?raw=true)

#### 🛠️ Core Architecture & Tech Stack
* **Backend API:** Go (Gin Framework, GORM) • JWT & OAuth 2.0 • PostgreSQL • OpenAPI/Swagger (Orval Client Generator)
* **Frontend Apps:** React • TanStack Query • Tailwind CSS • React Router
* **Cloud & Infrastructure:** Oracle Cloud VPS (Backend hosting) • Azure Static Web Apps (Frontend) • Azure API Management (API Gateway) • Azure Blob Storage (Media Asset Delivery) • Docker
* **CI/CD & DevOps:** GitHub Actions Automated Pipelines • Git

#### 🏗️ System Components & Engineering Highlights
* **Distributed Media Player:** A lightweight React-based engine deployed on edge OOH devices, optimized to pull scheduled playlists and cache/render media reliably.
* **Granular Content Scheduling:** Built a robust scheduling engine in Go to handle complex timeline logic, layout distribution, and device-oriented playlist delivery.
* **Production-Grade Infrastructure:**
  * Implemented an automated CI/CD pipeline via GitHub Actions that builds Docker containers and triggers production updates on every push.
  * Secured and rate-limited public endpoints using Azure API Management.
  * Optimized media serving costs and latency by decoupling file management into Azure Blob Storage.
* **Quality Assurance:** Covered with Unit, Integration, and End-to-End (E2E) automated tests to ensure zero-downtime deployments.

---

## 🛠️ Technical Toolkit

* **Languages:** Go (Golang), JavaScript/TypeScript, SQL
* **Backend Frameworks:** Gin Gonic, GORM
* **Messaging & Events:** Azure Service Bus, Event-Driven Architecture (EDA)
* **Frontend Tools:** React, TanStack Query, Tailwind CSS, React Router
* **Databases & Storage:** PostgreSQL, Azure Blob Storage
* **DevOps & Cloud:** Docker, Docker Compose, GitHub Actions, Oracle Cloud Infrastructure (OCI), Azure API Management, Azure Static Web Apps, Git
* **Architecture Patterns:** Monorepos, RESTful APIs, Event-Driven Processing, Inventory Decoupling, Eventual Consistency

---

📬 **How to reach me:** Feel free to connect via LinkedIn or open a discussion if you'd like to talk about full-stack architectures, Go backend optimization, or event-driven systems!
