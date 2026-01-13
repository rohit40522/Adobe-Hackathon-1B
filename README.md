# Adobe-Hackathon-1B

# 🗂️ Task Manager – Backend (Node.js & Express)

A RESTful backend API for a **Task Manager (Kanban) application** supporting
authentication, user management, task CRUD operations, and activity tracking.

---

## 📌 Project Overview

This backend provides secure APIs for:
- User authentication (JWT-based)
- User profile management
- Task creation, update, deletion
- Task filtering by status
- User-specific task isolation

It is designed to work with a React frontend using Axios.

---

## 🛠️ Tech Stack

- **Node.js**
- **Express.js**
- **MongoDB**
- **Mongoose**
- **JWT (JSON Web Tokens)**
- **bcrypt**
- **dotenv**

---

## 📁 Backend Folder Structure

```text
backend/
├── src/
│   ├── config/
│   │   └── db.js                # MongoDB connection
│   │
│   ├── models/
│   │   ├── User.js              # User schema
│   │   └── Task.js              # Task schema
│   │
│   ├── middleware/
│   │   └── auth.middleware.js   # JWT authentication middleware
│   │
│   ├── controllers/
│   │   ├── auth.controller.js   # Signup, login, logout
│   │   ├── user.controller.js   # Profile update & delete
│   │   └── task.controller.js   # Task CRUD logic
│   │
│   ├── routes/
│   │   ├── auth.routes.js       # Auth routes
│   │   ├── user.routes.js       # User routes
│   │   └── task.routes.js       # Task routes
│   │
│   ├── app.js                   # Express app configuration
│   └── server.js                # Server entry point
│
├── .env                         # Environment variables
└── package.json                 # Dependencies & scripts

