# Expense Tracker Dashboard - Personal Finance Management System

## 🔗 Live Demo
Access the live application here: **[https://expense-tracker-dashboard-ebon.vercel.app](https://expense-tracker-dashboard-ebon.vercel.app)**

Expense Tracker Dashboard is a full-stack personal finance management application built on the MERN stack (MongoDB, Express.js, React, Node.js). It provides users with secure authentication, real-time transaction tracking, automated budgeting insights, and clean data visualizations.

## 🚀 Key Features

* **Real-time Analytics:** Visual insights and graphs (Income vs. Expense breakdowns, category spending) using Recharts.
* **Transaction Management:** Complete CRUD functionality for adding, editing, deleting, and categorizing income and expenses.
* **Monthly/Yearly Budgeting:** Goal setting and automated warnings when spending approaches category thresholds.
* **JWT-Based Authentication:** Secure user registration, login, and protected routing.
* **Excel/CSV Export:** Export transaction data directly to xlsx spreadsheet format.

## 🛠️ Tech Stack

* **Front-End:** React.js, Vite, Tailwind CSS, Recharts, Axios, React Router Dom
* **Back-End:** Node.js, Express.js, MongoDB & Mongoose
* **Auth:** JSON Web Tokens (JWT), bcryptjs

---

## 💻 Local Setup & Execution

### Prerequisites
- Node.js (v18 or higher)
- MongoDB (running locally or Atlas connection string)

### 1. Clone & Set Up Directory
```bash
git clone https://github.com/NI3HIL/expense-tracker-dashboard.git
cd expense-tracker-dashboard
```

### 2. Back-End Configuration
Navigate to the `BackEnd` directory, install packages, and set up your `.env`:
```bash
cd BackEnd
npm install
```
Create a `.env` file in the `BackEnd` folder:
```env
PORT=5000
MONGODB_URI=mongodb://localhost/expense-tracker
JWT_SECRET=yoursecretkey
```
Start the backend server:
```bash
npm run dev
# Server will run on http://localhost:5000
```

### 3. Front-End Configuration
In a new terminal window, navigate to the `FrontEnd` directory, install packages, and start the development server:
```bash
cd FrontEnd
npm install
npm run dev
# App will run on http://localhost:5173
```

---

## 📄 License
This project is open-source and licensed under the MIT License.
