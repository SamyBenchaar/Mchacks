# MentorConnect - Professional Mentorship Platform

> **Note:** This repository is a **fork** of the original project developed during **McHacks 2025**. MentorConnect was built by a **team of four** during the hackathon. This fork is intended to showcase my individual contributions while preserving the original collaborative work.

## 🎯 Overview

MentorConnect is a full-stack web application that connects students with professional mentors through an intuitive platform designed to facilitate networking, mentorship, and career development.

## ✨ Key Features

- Secure authentication using JWT with Student and Mentor roles
- Mentor discovery with advanced search and filtering
- Real-time messaging powered by Socket.io
- Mentorship session booking (virtual and in-person)
- One-day job shadowing opportunities offered by mentors
- Smart recommendations based on user interests
- Personalized dashboards for each user
- Real-time notifications

---

# 🚀 Tech Stack

## Backend
- Node.js
- Express.js
- MongoDB Atlas
- Socket.io
- JWT Authentication
- Bcrypt

## Frontend
- React 18
- React Router v6
- Axios
- Socket.io Client
- Tailwind CSS

---

# 📦 Installation

## 1. Clone the repository

```bash
git clone <repository-url>
cd Mchacks
```

## 2. Install backend dependencies

```bash
cd backend
npm install
```

## 3. Install frontend dependencies

```bash
cd ../frontend
npm install
```

---

# ⚙️ Configuration

Before running the application, create the required `.env` files in both the **backend** and **frontend** directories.

### Backend (`backend/.env`)

```env
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
PORT=5000
```

### Frontend (`frontend/.env`)

```env
REACT_APP_API_URL=http://localhost:5000/api
REACT_APP_SOCKET_URL=http://localhost:5000
```

> **Note:** Environment files (`.env`) are intentionally **not included** in this repository for security reasons. You will need to provide your own MongoDB connection string and JWT secret before running the project.

---

# ▶️ Running the Application

## Start the backend (Terminal 1)

```bash
cd backend
npm run dev
```

The backend will be available at:

```
http://localhost:5000
```

## Start the frontend (Terminal 2)

```bash
cd frontend
npm start
```

The application will open at:

```
http://localhost:3000
```

---

# 👥 User Guide

## Students

1. Create a student account.
2. Complete your profile with your interests.
3. Browse and connect with mentors.
4. Chat with mentors in real time.
5. Schedule mentorship sessions.
6. Apply for one-day job shadowing opportunities.

## Mentors

1. Create a mentor account.
2. Complete your professional profile.
3. Set communication preferences.
4. Manage your availability.
5. Accept mentorship requests.
6. Offer optional one-day job shadowing opportunities.

---

# 📱 Application Pages

| Route | Description |
|--------|-------------|
| `/` | Home page |
| `/register` | User registration |
| `/login` | User login |
| `/dashboard` | Personalized dashboard |
| `/discover` | Browse mentors |
| `/messages` | Real-time messaging |
| `/internships` | Job shadowing opportunities |
| `/profile` | User profile management |

---

# 🗂 Project Structure

```
Mchacks/
├── backend/
│   ├── config/         # Database configuration
│   ├── models/         # Mongoose models
│   ├── routes/         # API routes
│   ├── controllers/    # Business logic
│   ├── middleware/     # Authentication & uploads
│   ├── utils/          # Utility functions
│   └── server.js       # Backend entry point
│
└── frontend/
    ├── public/
    └── src/
        ├── components/ # React components
        ├── pages/      # Main pages
        ├── contexts/   # Authentication & Socket contexts
        ├── services/   # API & Socket services
        └── App.jsx     # Frontend entry point
```

---

# 🎨 UI & Design

- Responsive interface
- Modern UI built with Tailwind CSS
- Accessible and user-friendly experience
- Consistent blue/indigo design system

---

# 🏆 Hackathon Highlights

During the hackathon, our team successfully implemented:

- Complete RESTful API
- Secure authentication system
- Real-time messaging
- Mentor discovery and recommendation features
- Session booking system
- Personalized dashboards
- Full-stack integration ready for demonstration

---

# 🛠 Troubleshooting

If you encounter issues:

1. Make sure your MongoDB instance is running and accessible.
2. Ensure ports **3000** and **5000** are available.
3. Clear the npm cache:

```bash
npm cache clean --force
```

4. Reinstall dependencies:

```bash
npm install
```

---

# 💻 Development

- The backend uses **nodemon** for automatic reloading.
- The frontend uses **React Scripts** with hot reloading.
- Run the backend and frontend simultaneously in separate terminals during development.

---

# 🎓 Built for McHacks 2025

MentorConnect was developed during **McHacks 2025**, one of Canada's largest hackathons. The project demonstrates the design and implementation of a full-stack mentorship platform built collaboratively by a team of four under hackathon time constraints.

---

**Happy hacking! 🚀**
