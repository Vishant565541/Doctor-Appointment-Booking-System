# LifeCare Full Stack Project

## Overview
LifeCare is a full-stack web application designed for healthcare management, featuring three main modules:
- **Frontend**: Patient-facing website
- **Admin**: Admin dashboard for managing doctors, patients, and appointments
- **Backend**: RESTful API server handling business logic and database operations

---

## Project Structure
```
lifecare-full-stack/
  ├── admin/      # Admin dashboard (React + Vite)
  ├── backend/    # Node.js/Express backend API
  └── frontend/   # Patient-facing frontend (React + Vite)
```

---

## How the Project Works

### 1. Frontend (Patient Website)
- Built with React and Vite.
- Allows patients to:
  - Register and log in
  - View doctors by specialty
  - Book appointments
  - View and manage their appointments
  - Update their profile
- Communicates with the backend via REST API calls.

### 2. Admin Dashboard
- Built with React and Vite.
- Allows admins to:
  - Log in securely
  - Add, edit, or remove doctors
  - View all appointments and patients
  - Manage doctor approvals and schedules
- Uses a separate context for admin authentication and state management.
- Communicates with the backend via REST API calls.

### 3. Backend (API Server)
- Built with Node.js, Express, and MongoDB.
- Handles authentication for users, doctors, and admins.
- Manages CRUD operations for users, doctors, and appointments.
- Integrates with Cloudinary for image uploads.
- Uses JWT for secure authentication.
- Provides separate routes for users, doctors, and admins.

---

## How to Run the Project

### Prerequisites
- Node.js (v16+ recommended)
- npm or yarn
- MongoDB instance (local or cloud)

### 1. Backend
```
cd backend
npm install
# Set up your environment variables (e.g., MongoDB URI, JWT secret, Cloudinary keys)
npm start
```
The backend server will start on the configured port (default: 5000).

### 2. Frontend (Patient Website)
```
cd frontend
npm install
npm run dev
```
The frontend will start on [http://localhost:5173](http://localhost:5173) by default.

### 3. Admin Dashboard
```
cd admin
npm install
npm run dev
```
The admin dashboard will start on [http://localhost:5174](http://localhost:5174) by default.

---

## Environment Variables
Each part of the project may require its own `.env` file. Example for backend:
```
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
```

---

## Features
- Patient registration, login, and profile management
- Doctor management by admin
- Appointment booking and management
- Secure authentication for all roles
- Responsive UI for both patients and admins

---

## Tech Stack
- **Frontend/Admin**: React, Vite, Tailwind CSS
- **Backend**: Node.js, Express, MongoDB, Cloudinary

---

## Contributing
Feel free to fork this repository and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

---

## License
This project is licensed under the MIT License. 