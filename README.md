# Hi there 👋

I'm a **Software Developer** focused on building full-stack applications, backend systems, and production-ready software.

I enjoy turning ideas into real products, working across the entire development lifecycle — from designing and developing applications to testing, deployment, and infrastructure.

> 🔒 **Corporate & Proprietary Software:** Due to software ownership and confidentiality restrictions, my core commercial projects are hosted in private repositories. Below, you can find the production-ready applications and proprietary SaaS platforms I have designed, built, and deployed independently.

---

## 🚀 Live SaaS Products & Applications

### 🛠️ Artisan Platform (AI-Driven Conversational ERP)
A multi-service **Conversational ERP monorepo** designed to transform natural language into structured business operations. Built specifically for non-tech-savvy artisans (e.g., crochet creators), the platform abstracts complex ERP interfaces entirely behind a **WhatsApp chat interface**.

The system utilizes an AI agent to interpret raw speech/text, resolve linguistic references, and interact with a strict domain API, ensuring AI is never the direct source of truth.

* **🌐 Conversational Interface:** Operating via WhatsApp API Webhooks.
* **🔧 Tech Stack:** Go (Gin Framework, GORM) • PostgreSQL • LLM APIs • Docker & Docker Compose
* **🌐 Web Admin Control:** React Dashboard *(Under development for metrics visual tracking)*

#### 🏗️ System Architecture & Data Flow
To ensure data integrity, the system is strictly split into decoupled layers:

WhatsApp Client -> **Intake Orchestrator (Go)** -> LLM API (Structured JSON)
* The Orchestrator then validates and sends an HTTP REST request to:
**Core Domain API (Go)** -> **PostgreSQL Database**

#### 🧠 Service Breakdown & Engineering Highlights
* **intake-orchestrator/ (Go + Gin):** Handles WhatsApp webhooks, chat context state management, idempotency controls, and prompts external LLMs. It forces the AI to output strict structured JSON schemas, detects missing transaction details, and translates backend responses back into conversational natural language.
* **api/ (Go + Gin + GORM):** The single source of truth and the only layer authorized to connect to PostgreSQL. It handles multi-tenant domain rules for Customers, Materials, Stock Movements, Orders, Sales, and Costs.
* **Decoupled AI Pattern:** The LLM *interprets* intent, the Orchestrator *coordinates*, the Domain API *validates/decides*, and PostgreSQL *persists*. This prevents AI hallucinations from corrupting financial or inventory data.

---

### 📺 Panel Management App (OOH Media Platform)
A full-stack **Out-of-Home (OOH) media management platform** designed to orchestrate and stream digital advertising content across distributed physical panels. 

I designed and engineered this entire platform end-to-end—building the high-performance Go API, the admin control center, and the edge media player that runs on connected physical hardware.

* **🌐 Live Production App:** [Link to your App here]
* **🔑 Guest/Demo Access:** **Username:** `demo@example.com` | **Password:** `Demo1234`
* **⚡ Media Player Instance:** [Link to player instance]

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
* **Frontend Tools:** React, TanStack Query, Tailwind CSS, React Router
* **Databases & Storage:** PostgreSQL, Azure Blob Storage
* **DevOps & Cloud:** Docker, Docker Compose, GitHub Actions, Oracle Cloud Infrastructure (OCI), Azure API Management, Azure Static Web Apps, Git
* **Architecture Patterns:** Monorepos, RESTful APIs, LLM Orchestration, Conversational UIs, Micro-services decoupling

---

📬 **How to reach me:** Feel free to connect via LinkedIn or open a discussion if you'd like to talk about full-stack architectures, Go backend optimization, or AI orchestration!
