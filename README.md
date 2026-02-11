# clearSKY ☁️  
**Academic Grading as a Service**

clearSKY is a modern **Software-as-a-Service (SaaS)** platform designed to streamline the academic grading workflow for educational institutions.  
It enables instructors to publish grades, manage review requests, and finalize submissions efficiently, while offering students transparency and structured feedback.

Developed as part of the **NTUA ECE SaaS 2025** course project.

---

## ✨ Key Features

### For Instructors
- Upload initial grades using standardized Excel templates
- Manage grade review requests in a structured workflow
- Publish final grades securely
- View grading statistics per course

### For Students
- View published grades
- Submit grade review requests
- Track instructor responses
- Access anonymized grade statistics

### For Institutions
- User and role management
- Credit-based usage model
- Centralized course oversight

---

## 🧱 Architecture Overview

clearSKY follows a **microservices architecture**, fully containerized and orchestrated using Docker.

- **Backend:** Node.js, SQL
- **Frontend:** React + TypeScript
- **Communication:** RabbitMQ (asynchronous message passing)
- **Authentication:** OAuth (Google Login)
- **Deployment:** Docker & Docker Compose

A detailed architectural diagram is available in the `architecture/` folder (Visual Paradigm).

---

## 🔌 Microservices

| Service | Description |
|------|------------|
| **AuthService** | Authentication and authorization |
| **CoursesService** | Course and enrollment management |
| **GradingService** | Grade handling and review workflow |
| **StatisticsService** | Grade analytics and statistics |
| **UserManagementService** | User roles and institution management |
| **Frontend** | React-based web interface |

---

## 🚀 Getting Started

### Prerequisites
- Docker
- Docker Compose

### Installation

```bash
git clone https://github.com/ntua/saas25-14.git
cd saas25-14
docker compose up --build


