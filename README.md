# Codolio 🚀

Codolio is a **LeetCode-inspired online coding platform** where users can solve programming problems and execute code in multiple languages using the **Judge0 API**.  
The project focuses on **secure code execution, role-based authorization, and scalable backend design**.

---

## 🔑 Key Features

- ✍️ Online code editor with multi-language support  
- ⚙️ Asynchronous code execution using Judge0  
- 📄 Execution results (output, runtime error, TLE, compilation error)  
- 🔐 User authentication & authorization (JWT-based)  
- 🧑‍💼 **Admin panel** for problem management  
- 📦 Submission handling & tracking  

---

## 🧑‍💼 Authentication & Authorization

- Users must be **authenticated** to submit solutions  
- **Role-based access control** is implemented:
  - 👤 **Normal users** can view and solve problems
  - 🛡️ **Only admins can add, update, or delete problems**
- Authorization is enforced using **middleware** on protected routes

---

## 🏗️ System Architecture


---

## 🔁 Code Execution Flow

1. User writes code and selects a language  
2. Frontend sends code to backend  
3. Backend forwards request to Judge0  
4. Judge0 returns a submission token  
5. Backend polls Judge0 asynchronously  
6. Final result is sent back to frontend  

---

## 🛠️ Tech Stack

**Frontend**
- React
- JavaScript
- HTML, CSS

**Backend**
- Node.js
- Express.js
- MongoDB
- Redis (for caching / queues)
- Judge0 API

**Languages Supported**
- C
- C++
- Java
- JavaScript  
*(Extendable via Judge0)*

---

## 🔐 Security Considerations

- Code is **never executed on the backend server**
- Judge0 provides **isolated sandboxed execution**
- API routes are protected using authentication middleware
- Environment variables and secrets are stored in `.env` files

---

## 🚀 Local Setup

```bash
# Backend
cd backend
npm install
npm run dev

# Frontend
cd frontend
npm install
npm start
