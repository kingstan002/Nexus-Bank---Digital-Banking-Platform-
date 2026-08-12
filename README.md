# 🏦 Nexus Bank – Full-Stack Secure Banking Platform

Nexus Bank is a **secure, full-stack digital banking application** built with Spring Boot and PostgreSQL. It demonstrates enterprise-grade architecture, JWT-based security, SOLID principles, and AI-driven user activity tracking with a 24-hour auto-cleanup policy for data privacy.

![Nexus Bank Dashboard](screenshot-dashboard.png)  
*(Replace with an actual screenshot of your dashboard)*

---

## 🚀 Live Demo (Optional)
> *If you have deployed it, add a link here. Example:*  
> [Live Demo](https://nexus-bank.onrender.com)

---

## ✨ Key Features

### 🔐 Security & Authentication
- **JWT-based stateless authentication** with BCrypt password hashing.
- Role-based access control (`USER` / `ADMIN`) to protect sensitive endpoints.
- JWT secret stored securely via **environment variables** (production-ready).

### 💰 Banking Core Logic
- Real-time **balance calculation** from transaction history.
- Support for **positive (deposits)** and **negative (withdrawals)** amounts.
- Full CRUD operations for user profiles and transactions.

### 📊 Dynamic Dashboard
- Beautiful, responsive **glassmorphism UI** built with HTML, CSS, and JavaScript.
- Displays live **balance**, **recent transactions**, and user profile.
- Connects to backend via secure **REST APIs** with JWT token management.

### 🤖 AI & Activity Tracking
- **User activity tracking** across channels (e.g., `LOGIN`, `TRANSACTION`, `PAYMENT`).
- `satisfied` flag logic to mark successful vs. failed actions.
- **24-hour auto-cleanup scheduler** that deletes satisfied activities daily at 2 AM for GDPR/Compliance.

### 🏗️ SOLID Architecture
- Built with **SOLID principles**:
  - `Single Responsibility`: Separation of Controllers, Services, Repositories.
  - `Open/Closed`: Interfaces like `IUserService`, `ITransactionService` for easy extension.
  - `Liskov Substitution`: Inheritance via `BaseUser`.
  - `Interface Segregation`: Fine-grained interfaces for each service.
  - `Dependency Inversion`: Controllers depend on interfaces, not concrete classes.

---

## 🛠️ Tech Stack

| Layer | Technology |
| :--- | :--- |
| **Backend** | Java 21, Spring Boot 4, Spring Security, JWT, Spring Data JPA |
| **Database** | PostgreSQL |
| **Frontend** | HTML5, CSS3, JavaScript (Vanilla), Chart.js |
| **Tools** | Maven, IntelliJ IDEA, Postman, pgAdmin |
| **Security** | BCrypt, JWT (JJWT), Environment Variables |
| **DevOps Ready** | Docker, Environment-based configuration |

---

## 📁 Project Structure (Simplified)
