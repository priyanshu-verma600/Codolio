# Codolio 🚀

Codolio is a **LeetCode-inspired online coding platform** where users can solve programming problems and execute code in some particular languages using the **Judge0 API**.  
The project focuses on **secure code execution, role-based authorization, and scalable backend design**.

---

## 🔑 Key Features

- ✍️ Online code editor with java, c++, javascript support  
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



