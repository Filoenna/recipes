# Recipes App

## Overview
A full-stack application with:
- **Backend:** FastAPI + SQLAlchemy (PostgreSQL)
- **Frontend:** Vue 3 (Composition API) + Tailwind CSS + DaisyUI
- **Database:** PostgreSQL
- **Containerization:** Docker & Docker Compose

## Getting Started

### Prerequisites
- Docker & Docker Compose installed

### Running the App
1. Navigate to the `app` directory:
   ```sh
   cd app
   ```
2. Build and start all services:
   ```sh
   docker-compose up --build
   ```
3. Access the frontend at [http://localhost:5173](http://localhost:5173)
4. Access the backend at [http://localhost:8000/docs](http://localhost:8000/docs)

---

- The backend connects to the database using the `DATABASE_URL` environment variable.
- The frontend is styled with Tailwind CSS and DaisyUI.
