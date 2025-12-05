# Project Management Tool

A robust and efficient **Project Management Application** designed to streamline **team collaboration**, **task tracking**, and **project planning**.  
This solution uses a **decoupled architecture** with separate **Frontend** and **Backend** repositories for better scalability and maintainability.

---

## Repository Structure

This project consists of two main components:

### ** Frontend**
- Handles the **User Interface** and all **client-side logic**  
- Repository: `project-management-frontend`

### ** Backend**
- Contains the **API server**, **database connection**, and **business logic**  
- Repository: `project-management` (Backend code is inside the `backend/` directory)

---

##  Tech Stack

### **Frontend**
- React.js  
- Axios  
- Styled Components / CSS / Tailwind (update based on your project)  

### **Backend**
- Node.js  
- Express.js  
- MongoDB / Mongoose  
- JWT Authentication  

*(Update icons or names above based on your exact technologies)*

---

##  Features

###  **User Authentication**
- Secure Login & Registration  
- JWT / Session-based authentication  

###  **Project Dashboard**
- Create, update, delete projects  
- View project lists and details  

###  **Task Management**
- Add tasks to projects  
- Assign tasks to members  
- Set due dates and priorities  

###  **Progress Tracking**
- Status indicators:  
  - **To Do**  
  - **In Progress**  
  - **Completed**  

###  **Team Collaboration**
- Add and manage team members  
- Assign roles and permissions  

###  **Responsive Design**
- Fully optimized for **desktop** and **mobile**  

---

##  Getting Started

Follow these steps to set up the project locally.

---

##  Prerequisites

Ensure you have the following installed:

- **Node.js** (v14 or higher)
- **npm** or **yarn**
- **MongoDB** (Local instance or Atlas URI)

---

#  1. Backend Setup

The backend manages the API and database.

```bash
# Clone the backend repository
git clone https://github.com/yourusername/project-management.git

# Navigate to backend directory
cd project-management/backend

# Install dependencies
npm install

# Create environment variables
# Inside backend/.env add:
# PORT=5000
# MONGO_URI=your_mongodb_connection_string
# JWT_SECRET=your_secret_key

# Start the server
npm start

# OR for development with nodemon
npm run dev

