# 🛠️ Incident Management System

A full-stack Incident Management System built with **Spring Boot 3** and **React 19**, designed with a production-ready architecture (JWT authentication, event-driven notifications, CI/CD, analytics dashboard).

---

## 🚀 Live Demo

🌐 Frontend: https://gestion-incidents-frontend.vercel.app  
🔗 Backend API: deployed on Render  
📖 API Docs: `/swagger-ui.html`

---

## 📦 Repositories

| Part     | Stack                          | Link                                                                 | Deployment |
|----------|--------------------------------|----------------------------------------------------------------------|------------|
| Backend  | Spring Boot 3, MySQL, JWT      | https://github.com/kaoutar629/GestionIncidents-backend              | Render     |
| Frontend | React 19, Vite, Tailwind       | https://github.com/kaoutar629/GestionIncidents-frontend             | Vercel     |

---

## ✨ Features

### 🔐 Authentication & Security
- JWT-based authentication (stateless)
- BCrypt password encryption
- Role-based access control (ADMIN / USER)

### 📋 Incident Management
- Create, update, delete incidents
- Status, priority, and category management
- Assignment of incidents to users

### 🤖 Intelligent Classification
- Rule-based classification engine (AI-inspired logic)
- Automatic suggestion of priority and category

### 📊 Analytics Dashboard
- Incident statistics visualization
- Charts (status distribution, priority trends)
- Data-driven insights

### 👥 Admin Features
- User management (ADMIN only)
- Role assignment and control

### 📧 Notifications
- Asynchronous email notifications
- Event-driven architecture (Spring Events)
- Mailtrap integration

### 🌙 UI/UX
- Dark / Light mode (persisted)
- Responsive design
- Modern UI with Tailwind + PrimeReact

---

## 🧠 Architecture Overview

- REST API architecture (decoupled frontend/backend)
- JWT-secured communication
- Clean layered architecture (Controller / Service / Repository)
- DTO-based API design
- Global exception handling for consistent responses

---

## ⚙️ Tech Stack

### Backend
- Spring Boot 3
- Spring Security + JWT
- Spring Data JPA (Hibernate)
- MySQL 8
- MapStruct
- Lombok
- Spring Events
- JavaMailSender
- SpringDoc (Swagger UI)

### Frontend
- React 19 + Vite
- Tailwind CSS
- React Router v7
- PrimeReact
- Chart.js
- React Toastify

---

## 🚀 CI/CD Pipeline

This project uses **GitHub Actions** for automation.

### Pipeline workflow:
- Backend build on every push
- Unit & integration tests execution
- Automatic deployment (Render / Vercel)

✔ Ensures continuous integration and reliable deployment.

---

## 🧪 Testing

### Backend tests:
- Authentication service (login, register, duplicate email handling)
- Business logic (incident classification, role-based deletion, validation rules)
- API integration tests using MockMvc

### Focus:
- Authentication flows
- Business rules validation
- API behavior consistency

---

## 🧱 Project Structure

### Backend

controller/
service/
security/
entity/
dto/
events/
mapper/
exception/


### Frontend

config/ → API client, auth, theme
components/ → reusable UI components
pages/ → dashboard, incidents, users
services/ → business logic
hooks/ → custom hooks
layout/ → application layout


---

## 🧠 Engineering Decisions

- Stateless JWT authentication for scalability
- Event-driven notifications for async processing
- DTO layer for clean API contracts
- Rule-based classification (no external API dependency)
- Global exception handling for consistency
- CI/CD pipeline for production readiness

---

## 💡 What I Learned

Building features is easy.  
Designing a system that is **clean, scalable, and production-ready** is the real challenge.

---

## 👩‍💻 Author

**Kaoutar**  
GitHub: https://github.com/kaoutar629
