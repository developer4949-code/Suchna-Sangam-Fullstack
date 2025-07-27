# 🌐 Suchna Sangam – Fullstack Project

**Suchna Sangam** is a full-stack application developed to bridge the digital divide in remote and underserved communities by delivering critical information and public services. The platform facilitates **news delivery**, **government policy access**, **grievance redressal**, and more through a clean, responsive frontend and a secure backend powered by Firebase and Spring Boot.

---

## 📌 Project Highlights

- **🧠 Goal**: Empower offline communities with essential news, education, government updates, and grievance tracking.
- **📶 Connectivity Challenge**: Designed with the idea of operating under poor or no internet zones by caching and syncing.
- **👥 User Roles**: Operator and Bureaucrat with role-specific access and functionality.

---

## 🏗️ Tech Stack

### ✅ Backend
- **Java 21**
- **Spring Boot 3.4**
- **Firebase (Auth + Firestore)**
- **RESTful APIs**
- **Gradle**

### ✅ Frontend
- **HTML5**
- **CSS3**
- **Vanilla JavaScript**

---

## 🚀 Features

### 🔒 Authentication & User Management
- Firebase-based login and signup
- Role-based access (Operator / Bureaucrat)
- Secure endpoints

### 📰 Information Delivery
- District-based **News**, **Policies**, and **Alerts**
- Historical policy retrieval by district

### 📨 Grievance Redressal
- Operators submit grievances
- Bureaucrats can view grievances in their district
- Grievance tracking and status updates

### 📧 Notifications
- Email alerts for important events (configurable)

---

## 🧩 Project Structure

```
Suchna-Sangam-Fullstack/
├── suchna-sangam-backend/
│   └── suchna-sangam-main/Suchnasangam-new-branch/
│       └── src/main/resources/serviceAccountKey.json
├── suchna-sangam-frontend/
│   └── Suchnasangam-main-frontend/
│       ├── index.html
│       ├── s_login.html, s_signup.html
│       ├── b_.html, op_.html
│       ├── about.html, random_git.html
│       ├── *.css, *.js, assets/
```

---

## 🧪 Getting Started

### 🔧 Backend Setup

1. **Clone Repository:**
```bash
git clone <your-backend-repo-url>
```

2. **Navigate to Backend Directory:**
```bash
cd suchna-sangam-main/Suchnasangam-new-branch
```

3. **Add Firebase Service Account Key:**
Place your `serviceAccountKey.json` inside:
```
src/main/resources/
```

4. **Run the App:**
```bash
./gradlew bootRun
```

### 🌐 Frontend Setup

1. **Clone Repository:**
```bash
git clone <your-frontend-repo-url>
```

2. **Open the App in Browser:**
Navigate to:
```
Suchnasangam-main-frontend/Suchnasangam-main/index.html
```

---

## 📡 API Endpoints (Backend)

| Endpoint | Method | Description |
|----------|--------|-------------|
| /api/auth/signup | POST | User registration |
| /api/auth/login | POST | User login |
| /users/{userId} | GET | Get user details |
| /news/{genre} | GET | Get news by genre |
| /policies/{districtId}/history | GET | Fetch policy history |
| /grievances/{districtId} | POST | Submit grievance |
| /api/alerts/{districtName} | GET | Get district-level alerts |

---

## 👨‍💻 Usage Guide

Register/Login as either:

🧑‍💼 Operator (submits grievances)

🧑‍⚖️ Bureaucrat (views district grievances)

**Access:**
- News, alerts, policies for your district.
- Submit and track grievances.

**Frontend Pages:**
- `index.html`: Entry point
- `s_login.html`, `s_signup.html`: Authentication
- `b_*.html`: Bureaucrat dashboard
- `op_*.html`: Operator dashboard
- `about.html`: App information

---

## 🤝 Contribution

Contributions are welcome!

- Fork the repositories
- Create a new branch
- Submit a pull request

---

## 📄 License

This project is licensed under the MIT License.
