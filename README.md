# Task Manager - Practical 10

A full-stack Task Management application featuring a React (Vite) frontend, an Express & MongoDB backend API with caching and authentication, and Docker Compose setup.

## Project Structure

- `TaskManager-frontend/`: React frontend built with Vite.
- `TaskManagerAPI/`: REST API built with Node.js, Express, MongoDB/Mongoose, JWT auth, and in-memory caching.
- `docker-compose.yml`: Multi-container Docker setup for running Frontend, Backend, and MongoDB together.

## Quick Start with Docker

```bash
# 1. Create .env for backend if needed
Copy-Item TaskManagerAPI/.env.example TaskManagerAPI/.env

# 2. Build and start all services
docker compose up --build
```

- Frontend: http://localhost:5173
- Backend API: http://localhost:3000
- MongoDB: localhost:27017

## Running Locally Without Docker

### Backend:
```bash
cd TaskManagerAPI
npm install
# configure .env
npm start
```

### Frontend:
```bash
cd TaskManager-frontend
npm install
npm run dev
```
