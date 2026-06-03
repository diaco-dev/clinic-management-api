# Clinic Management System

A modular, scalable backend system for clinic operations including patient management, appointments, and clinical workflows.

The system is designed using **Domain-Driven Design (DDD)** principles with a **modular monolith architecture** that is ready for future microservice extraction.

---

## 🧠 Architecture Overview

- Modular Monolith (DDD-aligned)
- Service Layer Architecture
- Async Processing (Celery + Redis)
- Stateless API (JWT-based)
- Microservice-ready boundaries

📌 Full architecture details:
- [C4 Context](docs/architecture/c4-context.md)
- [C4 Container](docs/architecture/c4-container.md)
- [C4 Component](docs/architecture/c4-component.md)
- [C4 Deployment](docs/architecture/c4-deployment.md)
---

## ⚙️ Tech Stack

- Python 3.12
- Django / Django REST Framework
- PostgreSQL
- Redis
- Celery
- Docker / Docker Compose

---

## 🚀 Run Locally

```bash
docker compose up --build