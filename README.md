# 🚀 Project Management Application

A powerful, scalable, and responsive Project Management Tool designed to streamline collaboration, task tracking, and productivity. Built with a decoupled **MERN (MongoDB, Express, React, Node.js)** architecture, ensuring high performance and maintainability.

``` bash
username = mukul12345
password = mukul12345
```
![React](https://img.shields.io/badge/React-19.0-61DAFB?logo=react&logoColor=black)
![Vite](https://img.shields.io/badge/Vite-6.0-646CFF?logo=vite&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-4.0-06B6D4?logo=tailwindcss&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-v14+-339933?logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-5.0-000000?logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-6.0-47A248?logo=mongodb&logoColor=white)

---

## 🌟 Key Features

### 🔐 Authentication & Security
- **Secure Login & Registration**: Powered by JWT (JSON Web Tokens) and bcrypt for password hashing.
- **Role-Based Access Control (RBAC)**: Distinct interfaces and capabilities for **Admins** and **Users**.

### 📊 Dashboard & Visualization
- **Interactive Charts**: Visual breakdown of task progress and project status using `recharts`.
- **Task Status Tabs**: Easily filter tasks by To Do, In Progress, and Completed.
- **Greeting Display**: Personalized user experience.

### 📝 Task & Project Management
- **CRUD Operations**: Complete control to create, read, update, and delete tasks and projects.
- **Task Assignment**: precise assignment of tasks to team members.
- **Priority & Due Dates**: Manage deadlines and importance levels effectively.

### 📂 File Handling & Reports
- **File Attachments**: Upload and manage files related to tasks (using `multer`).
- **Excel Export**: Generate reports and export data to Excel (using `exceljs`).

### 🎨 Modern UI/UX
- **Responsive Design**: Mobile-first approach using **Tailwind CSS v4**.
- **Toast Notifications**: Real-time feedback using `react-hot-toast`.
- **Dynamic Icons**: Rich iconography integrated via `react-icons`.

---

## 🏗️ Architecture

This project follows a decoupled client-server architecture:

- **Frontend (`task-manager-frontend-main`)**: Single Page Application (SPA) built with React 19 + Vite.
- **Backend (`backend`)**: RESTful API built with Node.js + Express.js.

---

## 🛠️ Tech Stack

### **Frontend**
- **Framework**: React 19
- **Build Tool**: Vite
- **Styling**: Tailwind CSS v4
- **Routing**: React Router DOM v7
- **HTTP Client**: Axios
- **State/Data**: Context API (assuming based on folder structure) / Props
- **Utilities**: Moment.js (Dates), React Hot Toast (Notifications)

### **Backend**
- **Runtime**: Node.js
- **Framework**: Express.js v5
- **Database**: MongoDB (via Mongoose ODM)
- **Authentication**: JWT, BcryptJS
- **File Handling**: Multer (Uploads), ExcelJS (Reports)
- **CORS**: Enabled for cross-origin requests

---

## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine.

### Prerequisites
- **Node.js** (v14 or higher)
- **npm** or **yarn**
- **MongoDB** (Local instance or Atlas Connection String)

### 1️⃣ Backend Setup

1.  Navigate to the backend directory:
    ```bash
    cd project-management-website/backend
    ```

2.  Install dependencies:
    ```bash
    npm install
    ```

3.  **Environment Configuration**:
    Create a `.env` file in the `backend` root and add your variables. Example:
    ```env
    PORT=5000
    MONGO_URI=mongodb://localhost:27017/project_management_db
    JWT_SECRET=your_super_secret_key_here
    ```

4.  Start the server:
    ```bash
    npm run dev
    # or
    npm start
    ```
    *The server should run on `http://localhost:5000` (or your defined PORT).*

### 2️⃣ Frontend Setup

1.  Navigate to the frontend directory:
    ```bash
    cd project-management-website/task-manager-frontend-main
    ```

2.  Install dependencies:
    ```bash
    npm install
    ```

3.  Start the development server:
    ```bash
    npm run dev
    ```

4.  Open your browser and navigate to the URL shown (usually `http://localhost:5173`).

---

## 🛣️ API Endpoints (Overview)

| Route Prefix | Description |
| :--- | :--- |
| `/api/auth` | Login, Register, Token Validation |
| `/api/users` | User profile, Role management |
| `/api/tasks` | CRUD operations for Tasks |
| `/api/reports` | Data export and analytics |
| `/api/attachments` | File upload and retrieval |

---

## 🤝 Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request
