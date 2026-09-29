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
How to Run the Project Locally
1. Clone the Repository
git clone https://github.com/mgneropj/TeamTaskManager.git
cd TeamTaskManager
2. Install Backend Dependencies

Open the terminal in VS Code:

cd backend
npm install
3. Configure Environment Variables

Create a .env file inside the backend folder:

PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret

Replace your_mongodb_connection_string with your MongoDB Atlas connection string.

Example:

MONGO_URI=mongodb+srv://username:password@cluster.mongodb.net/TaskManager

Never commit your .env file or expose your MongoDB credentials.

4. Start the Backend

From the backend folder:

npm run dev

If npm run dev is not available, use:

npm start

The backend will run on:

http://localhost:5000
5. Install Frontend Dependencies

Open a new terminal in VS Code:

cd frontend
npm install
6. Start the Frontend
npm run dev

Vite will provide a local URL, usually:

http://localhost:5173

Open this URL in your browser.


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
