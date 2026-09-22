# Hi there 👋

I'm a **Software Developer** focused on building full-stack applications, backend systems, and production-ready software.

I enjoy turning ideas into real products, working across the entire development lifecycle — from designing and developing applications to testing, deployment, and infrastructure.

I also have experience working on **corporate and proprietary software projects**. Due to software ownership and confidentiality restrictions, I cannot publicly share those projects.

Below are some of the applications I have designed, developed, and delivered that I can share publicly.



## Projects


## Panel Management App

A full-stack **OOH (Out-of-Home) media management platform** designed to manage digital media displayed across physical advertising panels.

I designed and developed the platform as a complete system composed of a **Go backend API**, a **React-based administration dashboard**, and a **React media player** responsible for running scheduled content on connected devices.

### Architecture

- **Backend:** Go + Gin + GORM
- **Authentication:** JWT + OAuth 2.0
- **Database:** PostgreSQL
- **Administration Dashboard:** React
- **Media Player:** React
- **API Documentation:** OpenAPI + Swagger
- **API Client:** Orval-generated client
- **Media Storage:** Azure Blob Storage
- **API Management:** Azure API Management
- **Frontend Hosting:** Azure Static Web Apps
- **Backend Hosting:** Oracle Cloud VPS
- **Containerization:** Docker
- **CI/CD:** GitHub Actions
- **Version Control:** Git + GitHub

### Main Features

- Media management
- Playlist management
- Digital panel management
- Content scheduling
- Scheduled media playback
- Device-oriented media player
- Administrative dashboard
- REST API
- Authentication and authorization
- Media storage and delivery through Azure Blob Storage
- API management through Azure API Management
- OpenAPI/Swagger documentation

### System Components

The platform is composed of three main applications:

- `api/` — Go backend responsible for business logic, authentication, media, playlists, panels, scheduling, and API operations.
- `web/` — React administration dashboard used to manage the OOH network and its content.
- `player/` — React-based player deployed on OOH devices to retrieve and play scheduled media.

### Frontend

The administration interface uses:

- React
- TanStack Query
- React Router
- Tailwind CSS
- React Icons
- Orval for generating the API client from the OpenAPI specification

The frontend is deployed using **Azure Static Web Apps**.

### Backend

The backend API is built with:

- Go
- Gin
- GORM
- PostgreSQL
- JWT
- OAuth 2.0
- CORS
- Swagger/OpenAPI
- Logging

The API is deployed on an **Oracle Cloud VPS**, with **Azure API Management** used as the API management layer.

### Infrastructure

The production architecture uses cloud services for different parts of the platform:

- **Oracle Cloud VPS** — backend API hosting
- **Azure Static Web Apps** — frontend hosting
- **Azure API Management** — API gateway and management
- **Azure Blob Storage** — storage for media assets
- **Docker** — application containerization
- **GitHub Actions** — CI/CD

### Testing & Engineering

The project includes:

- Unit tests
- Integration tests
- End-to-end tests
- OpenAPI-based API documentation
- Docker-based development
- CI/CD pipelines
- Git-based version control

### My Role

I designed and developed the platform end-to-end, covering the **backend API, administration dashboard, media player, database integration, authentication, media storage, API management, testing, deployment, containerization, and CI/CD infrastructure**.

