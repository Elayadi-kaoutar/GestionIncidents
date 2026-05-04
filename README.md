🛠️ Incident Management System

A full-stack Incident Management System built with Spring Boot 3 and React 19, designed with a production-like architecture (JWT auth, event-driven notifications, CI/CD, analytics dashboard).

🚀 Live Demo

🌐 Frontend: https://gestion-incidents-frontend.vercel.app

🔗 Backend API: deployed on Render
📖 API Docs: /swagger-ui.html

📦 Repositories
Part	Stack	Link	Deployment
Backend	Spring Boot 3, MySQL, JWT	https://github.com/kaoutar629/GestionIncidents-backend
	Render
Frontend	React 19, Vite, Tailwind	https://github.com/kaoutar629/GestionIncidents-frontend
	Vercel
✨ Key Features
🔐 Authentication & Security
JWT-based authentication (stateless)
BCrypt password encryption
Role-based access control (ADMIN / USER)
📋 Incident Management
Full CRUD operations
Status, priority, category management
Assignment of incidents to users
🤖 Intelligent Classification
Rule-based classification engine (AI-inspired logic)
Automatic suggestion of priority & category in real time
📊 Analytics Dashboard
Incident statistics visualization
Charts (status distribution, priority trends)
Data-driven overview for decision making
👥 Admin Features
User management (ADMIN only)
Role assignment and access control
📧 Notifications System
Asynchronous email notifications
Spring Events-driven architecture
Mailtrap integration
🌙 UI/UX
Dark / Light mode (persisted)
Responsive design
Modern UI with Tailwind + PrimeReact
🧠 Architecture Overview
REST API architecture (frontend ↔ backend decoupled)
Secure communication via JWT
Clean separation of layers (Controller / Service / Repository)
DTO-based API contracts
Global exception handling for consistent responses
⚙️ Tech Stack
Backend
Spring Boot 3
Spring Security + JWT
Spring Data JPA (Hibernate)
MySQL 8
MapStruct
Lombok
Spring Events
JavaMailSender
SpringDoc (Swagger UI)
Frontend
React 19 + Vite
Tailwind CSS
React Router v7
PrimeReact
Chart.js
React Toastify
🚀 CI/CD Pipeline

This project uses GitHub Actions for automation.

Pipeline includes:
Build backend on every push
Run unit & integration tests
Deploy backend (Render)
Deploy frontend (Vercel)

👉 Ensures continuous delivery and production reliability.

🧪 Testing Strategy
Backend tests:
AuthService (login, register, duplicate email validation)
IncidentService (business rules, classification, role-based deletion)
AuthController (integration tests with MockMvc)
Coverage focus:
Authentication flows
Business logic validation
API behavior consistency
🧱 Project Structure
Backend
controller/
service/
security/
entity/
dto/
events/
mapper/
exception/
Frontend
config/        → API client, auth, theme
components/    → reusable UI components
pages/         → dashboard, incidents, users
services/      → business logic (classification)
hooks/         → custom hooks
layout/        → UI structure
🧠 Engineering Decisions
Stateless JWT authentication → scalability
Event-driven notifications → non-blocking architecture
DTO layer → clean API contracts
Rule-based classification → no external API dependency
Global exception handling → consistent API responses
CI/CD automation → production-ready workflow
💡 What I Learned

This project helped me understand that:

Building features is easy.
Designing systems that are scalable, clean, and production-ready is the real challenge.

👩‍💻 Author

Kaoutar
GitHub: https://github.com/kaoutar629
