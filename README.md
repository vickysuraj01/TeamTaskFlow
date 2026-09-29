# 🚀 Team Task Manager

A full-stack **MERN (MongoDB, Express.js, React.js, Node.js)** application for managing team projects and tasks with JWT authentication, role-based access control, dashboard analytics, and project/task management.

---

## 📌 Features

### 🔐 Authentication

- User Registration
- User Login
- JWT Authentication
- Protected Backend Routes
- Password Hashing using bcrypt
- Logout

### 📁 Project Management

- Create Projects
- View Projects
- Edit Projects
- Delete Projects
- Project descriptions
- Project and user relationships

### ✅ Task Management

- Create Tasks
- Assign Tasks to Projects
- Set Task Priority
  - High
  - Medium
  - Low
- Update Tasks
- Delete Tasks
- Track Task Status
- View task project information

### 📊 Dashboard

- Total Projects
- Total Tasks
- Pending Tasks
- Recent Projects
- Recent Tasks
- Task Status Pie Chart
- Dashboard statistics from backend API

### 👥 Role-Based Access

The application supports two roles:

- **Admin**
- **Member**

Administrative operations such as creating, updating, and deleting projects are protected using role-based authorization.

---

# 🛠 Tech Stack

## Frontend

- React.js
- React Router DOM
- Axios
- Recharts
- React Hot Toast
- Tailwind CSS
- Vite

## Backend

- Node.js
- Express.js
- JWT Authentication
- bcrypt
- Mongoose
- CORS
- dotenv

## Database

- MongoDB Atlas
- Mongoose

---

# 📂 Project Structure

```text
TeamTaskManager/
│
├── backend/
│   ├── config/
│   │   └── db.js
│   │
│   ├── controllers/
│   │   ├── authController.js
│   │   ├── dashboardController.js
│   │   ├── projectController.js
│   │   └── taskController.js
│   │
│   ├── middleware/
│   │   └── authMiddleware.js
│   │
│   ├── models/
│   │   ├── User.js
│   │   ├── Project.js
│   │   └── Task.js
│   │
│   ├── routes/
│   │   ├── authRoutes.js
│   │   ├── dashboardRoutes.js
│   │   ├── projectRoutes.js
│   │   └── taskRoutes.js
│   │
│   ├── server.js
│   └── package.json
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   └── App.jsx
│   │
│   ├── vite.config.js
│   └── package.json
│
├── screenshots/
│   ├── login.png
│   ├── dashboard.png
│   ├── projects.png
│   └── tasks.png
│
├── .gitignore
└── README.md
