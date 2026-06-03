# Clinic Management System

> Backend infrastructure for a modern clinic management platform built with Django and scalable service-oriented architecture principles.

## Status

This project is currently under active development.

---

# Overview

Clinic Management System is a backend-focused healthcare platform designed to support clinic operations such as authentication, appointment management, patient workflows, notifications, and future financial integrations.

The system is built with scalability, modularity, and production-oriented architecture in mind.

---

# Core Features

* JWT Authentication
* Custom User Model with UUID Primary Keys
* PostgreSQL Database Integration
* Redis Caching & Queue Support
* Dockerized Development Environment
* Environment-Based Configuration
* CORS & CSRF Security Configuration
* SMS Service Integration Ready
* Payment Gateway Integration Ready
* Celery Background Task Support
* Modular Django App Structure

---

# Technology Stack

| Category         | Technology              |
| ---------------- | ----------------------- |
| Language         | Python 3.12             |
| Framework        | Django                  |
| Database         | PostgreSQL              |
| Cache / Queue    | Redis                   |
| Containerization | Docker & Docker Compose |
| Authentication   | JWT                     |
| Async Tasks      | Celery                  |

---

# Project Structure

```txt
.
├── core/
├── users/
├── appointments/
├── requirements/
├── docker/
├── manage.py
├── docker-compose.yml
├── Dockerfile
├── entrypoint.sh
└── .env
```

---

# Environment Configuration

Create a `.env` file based on `.env.sample`.

Example:

```env
DJANGO_SECRET_KEY=your-secret-key
DEBUG=True

POSTGRES_DB=clinic_db
POSTGRES_USER=postgres
POSTGRES_PASSWORD=postgres
POSTGRES_HOST=127.0.0.1
POSTGRES_PORT=5432

REDIS_HOST=127.0.0.1
REDIS_PORT=6379
```

---

# Running the Project

## Build and Start Containers

```bash
docker compose up --build
```

---

# Useful Commands

## Create Superuser

```bash
docker compose exec web python manage.py createsuperuser
```

## Run Database Migrations

```bash
docker compose exec web python manage.py migrate
```

## Open Django Shell

```bash
docker compose exec web python manage.py shell
```

---

# Development Roadmap

Planned modules and integrations:

* Appointment Management
* Doctor Scheduling
* Patient Medical Records
* Prescription System
* Notification Service
* Audit Logging
* Payment Processing
* Role-Based Access Control
* API Documentation
* Automated Testing
* CI/CD Pipeline

---

# Architecture Notes

* UUID is used for primary keys across the system.
* PostgreSQL and Redis run in isolated containers.
* Environment variables are used for all sensitive configuration.
* The project is structured for scalability and modular expansion.

---

# License

This project is licensed under the MIT License.

