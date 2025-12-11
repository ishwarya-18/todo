# Task Manager Application

A modern, full-stack task management application built with React and Node.js.

## 🚀 Live Demo

- **Frontend**: Deployed on Render
- **Backend**: [[https://todo-app-bzwv.onrender.com](https://todo-backend-gyqk.onrender.com)](https://todo-backend-gyqk.onrender.com)

## ✨ Features

- **User Authentication**: Secure login and signup with JWT tokens
- **Task Management**: Create, complete, and delete tasks
- **Admin Panel**: Manage users and promote to admin role
- **Dark/Light Theme**: Toggle between themes
- **Responsive Design**: Works on desktop and mobile devices

## 🛠️ Tech Stack

### Frontend
- React 18
- TypeScript
- Vite
- Tailwind CSS
- Shadcn/UI Components
- React Router DOM
- TanStack Query

### Backend
- Node.js
- Express.js
- PostgreSQL
- JWT Authentication
- bcryptjs for password hashing

## 📁 Project Structure

```
├── backend/                 # Node.js backend
│   ├── server.js           # Express server and API routes
│   ├── package.json        # Backend dependencies
│   └── .env                # Environment variables
├── src/                    # React frontend
│   ├── components/         # Reusable UI components
│   ├── contexts/           # React contexts (Auth, Theme)
│   ├── pages/              # Page components
│   ├── lib/                # Utilities and API functions
│   └── hooks/              # Custom React hooks
└── public/                 # Static assets
```

## 🚀 Getting Started

### Prerequisites

- Node.js 18+
- PostgreSQL database
- npm or yarn

### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file with:
   ```env
   DATABASE_URL=your_postgresql_connection_string
   JWT_SECRET=your_jwt_secret_key
   PORT=5000
   ```

4. Start the server:
   ```bash
   npm start
   ```

### Frontend Setup

1. Install dependencies:
   ```bash
   npm install
   ```

2. Create environment variable (optional):
   ```env
   VITE_API_URL=http://localhost:5000
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

## 🔗 API Endpoints

### Authentication
- `POST /auth/signup` - Register new user
- `POST /auth/login` - Login user

### Tasks
- `GET /todos` - Get all tasks (authenticated)
- `POST /todos` - Create new task
- `PATCH /todos/:id` - Toggle task completion
- `DELETE /todos/:id` - Delete task

### Users (Admin only)
- `GET /users` - Get all users
- `DELETE /users/:id` - Delete user
- `PUT /users/:id/promote` - Promote user to admin

## 📄 License

This project is open source and available under the MIT License.
