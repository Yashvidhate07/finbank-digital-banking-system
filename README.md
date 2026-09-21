# 🏦 FinBank – Digital Banking Management System

A full-stack digital banking management system built with **Spring Boot, React.js, MySQL, Spring Data JPA, Hibernate, and JWT Authentication**.

FinBank provides a secure and user-friendly platform for managing banking operations such as user registration, authentication, accounts, transactions, and other digital banking services.

---

## 🚀 Features

### 🔐 Authentication & Security
- User registration and login
- JWT-based authentication
- Role-based access control
- Secure password handling
- Protected API endpoints
- Spring Security integration

### 👤 User Management
- Create and manage user accounts
- User profile management
- Account information
- Secure authentication and authorization

### 💳 Banking Operations
- Bank account management
- Deposit and withdrawal operations
- Fund transfers
- Transaction management
- Transaction history
- Account balance management

### 📊 Dashboard
- User banking dashboard
- Account overview
- Transaction information
- Banking activity tracking

### 🔗 REST APIs
- RESTful backend APIs
- Spring Boot controllers and services
- Spring Data JPA repositories
- MySQL database integration

---

## 🛠️ Tech Stack

### Frontend
- React.js
- JavaScript
- HTML5
- CSS3
- Vite

### Backend
- Java 17
- Spring Boot
- Spring Security
- Spring Data JPA
- Hibernate
- REST APIs
- JWT

### Database
- MySQL

### Development Tools
- Git
- GitHub
- Maven
- IntelliJ IDEA / VS Code
- Postman

---

## 🏗️ Project Architecture

```text
FinBank
│
├── backend
│   ├── src
│   │   └── main
│   │       ├── java
│   │       └── resources
│   ├── pom.xml
│   └── ...
│
├── frontend
│   ├── src
│   ├── public
│   ├── package.json
│   └── ...
│
├── .gitignore
└── README.md
```

The application follows a typical full-stack architecture:

```text
React Frontend
      │
      │ REST API / HTTP
      ▼
Spring Boot Backend
      │
      │ Spring Data JPA / Hibernate
      ▼
    MySQL
```

---

# ⚙️ Getting Started

## 1. Clone the Repository

```bash
git clone https://github.com/Yashvidhate07/finbank-digital-banking-system.git
```

Move into the project:

```bash
cd finbank-digital-banking-system
```

---

# 🗄️ Backend Setup

## 2. Create the MySQL Database

Open MySQL and run:

```sql
CREATE DATABASE banking_system;
```

---

## 3. Configure Database

The backend uses environment variables for database configuration.

Example:

```properties
spring.datasource.url=${DB_URL:jdbc:mysql://localhost:3306/banking_system?useSSL=false&serverTimezone=UTC}
spring.datasource.username=${DB_USERNAME:root}
spring.datasource.password=${DB_PASSWORD:your_password}

spring.jpa.hibernate.ddl-auto=update
```

Replace `your_password` with your local MySQL password.

> **Security:** Never commit real database passwords, JWT secrets, API keys, or other credentials to a public repository. GitHub recommends using repository security features and avoiding committed secrets.

---

## 4. Run the Spring Boot Backend

Navigate to the backend:

```bash
cd backend
```

Run:

```bash
mvn spring-boot:run
```

The backend runs on:

```text
http://localhost:8080
```

---

# 💻 Frontend Setup

Open another terminal.

Navigate to the frontend:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

The frontend will normally run on:

```text
http://localhost:5173
```

---

# 🔄 Application Flow

```text
User
 │
 ▼
React Frontend
 │
 │ HTTP Request
 ▼
Spring Boot REST API
 │
 ├── Spring Security
 │
 ├── JWT Authentication
 │
 ├── Controller
 │
 ├── Service
 │
 └── Repository
        │
        ▼
      MySQL
```

---

# 🔐 Authentication Flow

```text
User Login
    │
    ▼
React Frontend
    │
    ▼
Login API
    │
    ▼
Spring Security
    │
    ▼
Validate Credentials
    │
    ▼
Generate JWT
    │
    ▼
Return Token
    │
    ▼
Frontend Stores Token
    │
    ▼
Authenticated API Requests
```

---

# 🧪 API Testing

You can test backend REST APIs using:

- Postman
- Browser Developer Tools
- Frontend application

Backend base URL:

```text
http://localhost:8080
```

---

# 📌 Project Goals

The main goals of FinBank are:

- Build a complete full-stack banking application
- Implement secure authentication using JWT
- Practice Spring Boot REST API development
- Implement database operations using JPA/Hibernate
- Connect React with a Spring Boot backend
- Implement real-world banking workflows
- Follow layered backend architecture

---

# 🔮 Future Enhancements

Potential future improvements include:

- Email OTP verification
- Two-factor authentication
- Transaction notifications
- PDF bank statements
- Admin analytics dashboard
- Transaction search and filtering
- Improved account security
- Docker deployment
- Cloud deployment
- Automated CI/CD pipeline

---

# 👨‍💻 Author

**Yash Vidhate**

Computer Engineering Graduate  
Pune, Maharashtra, India

GitHub:  
https://github.com/Yashvidhate07

---

# 📄 License

This project is intended for educational and portfolio purposes.

---

## ⭐ Support

If you find this project useful, consider giving the repository a ⭐ on GitHub.
