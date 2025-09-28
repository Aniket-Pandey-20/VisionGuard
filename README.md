# VisionGuard – Real-Time Multi-Camera Face Detection Dashboard  

VisionGuard is a real-time, multi-camera monitoring dashboard that allows users to register IP/RTSP cameras, view live video streams, and receive instant face-detection alerts

---

## 🚀 Features
- 🔐 **JWT Authentication** – secure login with protected APIs  
- 🎥 **Camera Management** – add, list, update, and remove cameras  
- 📊 **Dashboard** – responsive grid layout for multiple camera tiles  
- ⚡ **Realtime Alerts** – face-detection alerts delivered via WebSocket  
- ▶️ **Start/Stop Controls** – toggle camera streams dynamically  
- 🗄️ **Database** – Prisma + PostgreSQL for persistence  
- 🛠️ **Simulated Worker** – generates alerts to demonstrate end-to-end flow  
- 🐳 **Dockerized** – run entire stack with one command  

---

## 📂 Tech Stack
- **Frontend:** React, TypeScript, Vite, MUI, Tailwind  
- **Backend:** Node.js, Hono/Express, JWT Auth, WebSockets  
- **Database:** PostgreSQL + Prisma ORM  
- **Worker:** (MVP) Node.js simulation; (Planned) Go + gocv/go-face + MediaMTX  
- **Deployment:** Docker, Docker Compose  

---

## 🔑 Demo Credentials
Use the following test account to log in:  
- **Email:** `test@visionguard.ai`  
- **Password:** `Test123!`  

---

## ⚡ Quick Start

### 1. Clone the repository
```bash
git clone https://github.com/yourname/visionguard.git
cd visionguard
```

### 2. Create a .env file in backend/:
Add below listed variables:
```bash
DATABASE_URL=postgresql://user:password@db:5432/visionguard
JWT_SECRET=supersecret
PORT=3000
```

### 3. Run with Docker Compose
```bash
  docker compose up --build
```
This will start the following services:
- **Backend API** → http://localhost:3000  
- **Frontend** → http://localhost:5173  
- **PostgreSQL Database**  
- **Worker** (simulated alerts)  
