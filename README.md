# clearSKY ☁️  
<img width="404" height="185" alt="image" src="https://github.com/user-attachments/assets/46a625e8-235f-43d8-9bde-3fa23b5a56f5" />

**Academic Grading as a Service**

clearSKY is a cloud‑native **Software‑as‑a‑Service (SaaS)** platform that modernizes the academic grading workflow for educational institutions.

It enables instructors to publish grades, manage structured review requests, and finalize submissions efficiently, while providing students with transparency, feedback, and statistical insights.

This project was designed and implemented as part of the **NTUA ECE – Software as a Service (2025)** course, following real‑world SaaS architectural practices.

---

## Problem Statement

Academic grading workflows are often:
- Manual and time‑consuming
- Poorly standardized across instructors
- Lacking transparency for students
- Difficult to scale institution‑wide

clearSKY addresses these issues by providing a **centralized, scalable, and asynchronous grading platform** that supports the full grading lifecycle.

---

## Core Features

### Instructors
- Upload initial grades using standardized Excel templates
- Manage grade review requests through a structured workflow
- Respond to student requests asynchronously
- Publish final grades securely
- View grading statistics per course

### Students
- View published grades
- Submit grade review requests
- Track instructor responses
- Access anonymized grade statistics

### Institutions
- User and role management
- Credit‑based usage model
- Centralized course oversight

---

## System Architecture

clearSKY is built using a **microservices architecture**, designed for scalability, fault isolation, and asynchronous communication.

### Architectural Highlights
- Service‑oriented backend
- Message‑based communication using RabbitMQ
- Stateless services
- Containerized deployment
- Clear separation of concerns

A detailed architecture diagram is available in the `architecture/` directory (Visual Paradigm).

---

## Microservices

| Service | Responsibility |
|------|----------------|
| **AuthService** | Authentication & authorization (OAuth) |
| **CoursesService** | Course and enrollment management |
| **GradingService** | Grade handling & review workflow |
| **StatisticsService** | Grade analytics and statistics |
| **UserManagementService** | User roles & institution management |
| **Frontend** | React‑based web interface |

---

## Technology Stack

### Backend
- Node.js
- SQL databases
- REST APIs
- RabbitMQ (asynchronous messaging)

### Frontend
- React
- TypeScript

### Infrastructure & DevOps
- Docker
- Docker Compose
- Microservice orchestration
- Message‑driven architecture

---

## 🚀 Running the Project Locally

### Prerequisites
- Docker
- Docker Compose

### Setup

```bash
git clone https://github.com/ntua/saas25-14.git
cd saas25-14
docker compose up --build
