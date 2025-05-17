# Flynkle Platform

Flynkle is your company's second brain – a platform of AI agents trained on your documents, connected to your tools, and capable of automating 80–90% of knowledge work across roles.

This monorepo organizes all core services and apps required to run the Flynkle ecosystem.

---

## 🧱 Architecture Overview

### Services

| Service           | Description                                    |
|------------------|------------------------------------------------|
| `flynkle-api`     | REST API Gateway that connects frontend to core services |
| `flynkle-brain`   | Ingestion, vector DB, chunking, RAG logic, Neo4j graph |
| `flynkle-auth`    | Authentication, email verification, user/session mgmt |
| `flynkle-web`     | Next.js frontend app                           |
| `flynkle-agents`  | (WIP) Specialized AI agents with tool usage    |
| `flynkle-reports` | (WIP) Reporting, analytics & dashboards        |
| `flynkle-shared`  | (Optional) Shared models/utilities between services |

---

## 🐳 Local Development (Docker Compose)

```bash
docker-compose up --build

## 📦 Project Structure
flynkle-platform/
├── flynkle-api/
├── flynkle-auth/
├── flynkle-brain/
├── flynkle-web/
├── flynkle-agents/   # optional
├── flynkle-reports/  # optional
├── docker-compose.yml
└── README.md

## 📬 Contact
For feedback, bugs, or ideas:
📧 noreply@flynkle.com
🌐 https://flynkle.com