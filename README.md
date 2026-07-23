# Hospital Appointment System

A modern hospital appointment management web application that allows patients to book appointments with doctors, doctors to manage profiles and availability, and administrators to oversee the system efficiently.

This project is built with a React frontend and an Express backend, connected to MongoDB for persistent data storage.

## Project Overview

The Hospital Appointment System provides a simple and user-friendly experience for:

- Patient registration and login
- Doctor registration and profile management
- Doctor discovery and filtering
- Appointment booking and management
- Profile image upload support
- Secure authentication using JWT

## Features

### Patient Features
- Register and log in securely
- View available doctors
- Book appointments
- View appointment history
- Update profile information

### Doctor Features
- Create and manage doctor profiles
- Set availability information
- View appointment requests
- Manage patient appointments

### General Features
- Responsive UI for desktop and mobile
- Dark/light theme support
- Protected routes for authenticated users
- RESTful API backend

## Tech Stack

### Frontend
- React
- Vite
- Tailwind CSS
- Axios
- React Router DOM

### Backend
- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT Authentication
- Multer for file uploads

## Project Structure

```bash
client/      # React frontend
server/      # Express backend
```

## Prerequisites

Make sure you have the following installed:

- Node.js (recommended latest LTS version)
- npm
- MongoDB database

## Installation

1. Clone the repository
2. Install dependencies for the root project, server, and client

```bash
npm run install-all
```

## Environment Variables

### Server
Create a `.env` file inside the `server` folder with the following variables:

```env
MONGO_URI=your_mongodb_connection_string
PORT=5000
JWT_SECRET=your_secret_key
```

### Client
Create a `.env` file inside the `client` folder if needed:

```env
VITE_API_URL=http://localhost:5000/api
```

For production deployment, update this value to your deployed backend URL.

## Running the Application Locally

### Start both frontend and backend

```bash
npm run dev
```

This will start:
- Frontend on the Vite dev server
- Backend on the Express server

### Start separately

```bash
npm run server
npm run client
```

## Build for Production

### Build the client

```bash
npm run build --prefix client
```

### Start the server

```bash
npm start --prefix server
```

## Deployment

The project is suitable for deployment on:

- Frontend: Vercel
- Backend: Render
- Database: MongoDB Atlas

### Recommended setup
- Deploy the backend on Render
- Deploy the frontend on Vercel
- Set the frontend environment variable:

```env
VITE_API_URL=https://your-render-backend-url/api
```

## Notes

- Ensure your backend has a valid MongoDB connection string.
- For production, configure CORS properly to allow your frontend domain.
- Profile image uploads require the uploads folder to be available on the server.

## License

This project is for educational and demonstration purposes.
