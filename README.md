# 🛠️ Gestion des Incidents

Système fullstack de gestion d'incidents, construit avec **Spring Boot 3** (backend) et **React 19** (frontend).

| Repo                                                              |Stack                     | Déployé sur |
|-------------------------------------------------------------------|--------------------------|-------------|
| [Backend](https://github.com/kaoutar629/GestionIncidents-backend) | Spring Boot 3, MySQL, JWT | Render |
| [Frontend](https://github.com/kaoutar629/GestionIncidents-frontend)| React 19, Vite, Tailwind | Vercel |

🌐 **Demo live :** [gestion-incidents-frontend.vercel.app](https://gestion-incidents-frontend.vercel.app)

---

## ✨ Fonctionnalités

- 🔐 Authentification JWT + BCrypt (rôles ADMIN / USER)
- 📋 CRUD incidents (statut, priorité, catégorie, assigné)
- 🤖 Classificateur IA maison — suggestion de priorité/catégorie en temps réel
- 📊 Dashboard analytique (doughnut + line chart)
- 👥 Gestion des utilisateurs (admin only)
- 📧 Notifications email asynchrones (Spring Events + Mailtrap)
- 🌙 Mode dark/light persisté
- 📖 Swagger UI disponible sur `/swagger-ui.html`

---

## 🚀 Lancer le projet en local

### Prérequis
- Java 21+, Maven 3.9+, MySQL 8+
- Node.js 18+, npm 9+

### Backend
```bash
git clone https://github.com/kaoutar629/GestionIncidents-backend.git
cd GestionIncidents-backend
# Configurer les variables d'environnement (voir README backend)
./mvnw spring-boot:run
# API : http://localhost:8080
# Swagger : http://localhost:8080/swagger-ui.html
```

### Frontend
```bash
git clone https://github.com/kaoutar629/GestionIncidents-frontend.git
cd GestionIncidents-frontend
npm install
# Créer .env.development avec : VITE_API_URL=http://localhost:8080/api
npm run dev
# App : http://localhost:5173
```

---

## 🧰 Tech Stack

### Backend
| Technologie | Usage |
|-------------|-------|
| Spring Boot 3 | Framework REST |
| Spring Security + JWT | Auth & sessions stateless |
| Spring Data JPA / Hibernate | ORM |
| MySQL 8 | Base de données |
| MapStruct + Lombok | Mapping & boilerplate |
| SpringDoc / Swagger UI | Documentation API |
| JavaMailSender + Spring Events | Notifications email async |

### Frontend
| Technologie | Usage |
|-------------|-------|
| React 19 + Vite 7 | UI & build |
| React Router v7 | Navigation |
| Tailwind CSS v4 | Styling |
| PrimeReact | Composants UI |
| Chart.js | Graphiques dashboard |
| React Toastify | Notifications toast |

---

## 📁 Structure du projet
GestionIncidents/
├── GestionIncidents-backend/    # API Spring Boot
│   └── src/main/java/.../
│       ├── controller/
│       ├── service/
│       ├── security/
│       ├── entity/ & dto/
│       ├── events/ & mappers/
│       └── exception/
│
└── GestionIncidents-frontend/   # App React
└── src/
├── config/       # API client, AuthContext, ThemeContext
├── components/   # Composants réutilisables
├── pages/        # Dashboard, Incidents, Users, Login
├── services/     # AiService (classification)
├── hooks/        # useAiClassifier, useIncidents
└── layout/       # Navbar, BodyContent

---

## 👩‍💻 Auteure

**Kaoutar** — [github.com/kaoutar629](https://github.com/kaoutar629)
