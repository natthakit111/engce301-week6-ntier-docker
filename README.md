# 🚀 Task Board - N-Tier Architecture (Docker + Railway)

## ENGCE301 - Week 7 Cloud Deployment Lab

---

## 👤 Student Information

- **Name:** ณัฐกิตติ์ ยั่งยืนปิยรัตน์  
- **Student ID:** 66543206014-3  

---

# 📌 Project Overview

This project demonstrates deployment of a **Task Board application** using **N-Tier Architecture** with **Docker** and **Cloud Platform (Railway)**.

The system is divided into three main layers:

- **Frontend** – Web interface for managing tasks  
- **Backend API** – REST API built with Node.js and Express  
- **Database** – PostgreSQL for storing task data  

---

# 🏗 System Architecture

Frontend (Browser)
│
▼
Backend API (Node.js / Express)
│
▼
PostgreSQL Database


All services are deployed on **Railway Cloud Platform**.

---

# 🌐 Live Deployment

| Service | URL |
|------|-----|
| Frontend | https://attractive-spirit-production-e8e6.up.railway.app |
| Backend API | https://engce301-week6-ntier-docker-production.up.railway.app |
| API Health Check | https://engce301-week6-ntier-docker-production.up.railway.app/api/health |
| Database | Internal (Railway PostgreSQL) |

---

# ✨ Features

- Create tasks
- Update task status
- Delete tasks
- Task statistics dashboard
- Priority management

---

# 🧰 Technology Stack

### Frontend
- HTML
- CSS
- JavaScript

### Backend
- Node.js
- Express.js
- REST API

### Database
- PostgreSQL

### Deployment
- Docker
- Railway Cloud Platform
- GitHub

---

# 🔗 API Endpoints

| Method | Endpoint | Description |
|------|------|------|
| GET | `/api/tasks` | Get all tasks |
| GET | `/api/tasks/:id` | Get task by ID |
| POST | `/api/tasks` | Create new task |
| PUT | `/api/tasks/:id` | Update task |
| DELETE | `/api/tasks/:id` | Delete task |
| GET | `/api/tasks/stats` | Get task statistics |
| GET | `/api/health` | API health check |


# 🐳 Running Locally with Docker

## Clone repository

```bash
git clone https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPOSITORY.git
cd YOUR_REPOSITORY
```
Start services
```
docker compose up -d
```
Access application

Frontend:
http://localhost:8080

Backend API:
http://localhost:3000/api

⚙ Environment Variables
```Example .env
DB_HOST=db
DB_PORT=5432
DB_NAME=taskboard_db
DB_USER=taskboard
DB_PASSWORD=password
NODE_ENV=development
PORT=3000
```


📂 Repository Structure
```
week6-ntier-docker/
│
├── api/                    # Backend API
│   ├── package.json
│   ├── server.js
│   └── src/
│
├── frontend/               # Frontend application
│   ├── index.html
│   ├── css/style.css
│   └── js/app.js
│
├── database/               # Database initialization
│   └── init.sql
│
├── screenshots/            # Deployment screenshots
│   ├── dashboard.png
│   ├── frontend.png
│   ├── api-health.png
│   ├── logs.png
│   └── metrics.png
│
├── docker-compose.yml
├── CLOUD_DEPLOYMENT.md
└── README.md
```