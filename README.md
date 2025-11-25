# 🎨 Animathics — Personal Portfolio + Projects + Competitions + YouTube Hub

Animathics is a full-stack personal website showcasing math, physics, coding, cybersecurity, and YouTube content in a clean, modern, highly scalable platform.
Built with Django + React + Vite + PostgreSQL + Tailwind, the site combines strong UI/UX with a structured backend suitable for long-term content growth.

This project acts as a unified home for:

About Me & Journey

Coding & Tech Projects

Coding Competitions & Rating Progress

YouTube Videos & Shorts

Future Animathics Articles & Blogs

## 🚀 Features
### 🔹 About Me

Bio, journey timeline, skills

Dynamic backend model for easy updates

Responsive design with animations

### 🔹 Projects

Full CRUD project system

Categories (Math, Coding, Cybersecurity, YouTube)

Tags & search filters

Featured Projects carousel

Individual project detail pages

### 🔹 Coding Competitions

Competition model (platform, rating, date, links)

Rating progress chart

Filters: platform, year, ranking

Achievement badge system

### 🔹 YouTube Integration

Automatic sync with YouTube Data API

Video grid with thumbnails

Shorts section

Embedded video player

Category filtering

### 🔹 Global Features

Minimal, modern React UI

Dark/Light mode toggle

Fully responsive

SEO optimized

Secure backend with rate limiting & CORS protection

## 🏗 Tech Stack
### Frontend

React

Vite

TailwindCSS

React Router

Chart.js / Recharts (rating progress)

### Backend

Django

Django REST Framework

PostgreSQL

django-environ

django-cors-headers

django-ratelimit

Infrastructure

Docker (frontend + backend)

GitHub Actions CI/CD

Render (Backend Deployment)

Vercel (Frontend Deployment)

## 📁 Project Structure
animathics/
│
├── backend/
│   ├── animathics_backend/
│   │   ├── settings/
│   │   │   ├── base.py
│   │   │   ├── dev.py
│   │   │   ├── prod.py
│   │   ├── core/
│   │   ├── api/
│   │   └── ...
│   ├── Dockerfile
│   └── manage.py
│
├── frontend/
│   ├── src/
│   ├── public/
│   ├── Dockerfile
│   └── vite.config.js
│
├── .github/workflows/
│   ├── backend-ci.yml
│   └── frontend-ci.yml
│
└── README.md

## ⚙️ Setup Instructions
### 1. Clone the Repository
git clone https://github.com/yourusername/animathics.git
cd animathics

## 🛠 Backend Setup (Django)
### 2. Install Environment & Dependencies
cd backend
pip install -r requirements.txt

### 3. Create Environment File
DEBUG=True
SECRET_KEY=your-secret
DATABASE_URL=postgres://user:pass@localhost:5432/animathics
ALLOWED_HOSTS=*
CORS_ALLOW_ALL_ORIGINS=True
YOUTUBE_API_KEY=your-api-key

### 4. Apply Migrations
python manage.py migrate

### 5. Start Backend
python manage.py runserver

## 🎨 Frontend Setup (React + Vite)
###6. Install Dependencies
cd frontend
npm install

### 7. Run Frontend
npm run dev

## 🐳 Docker Setup (Optional)
docker-compose up --build

## 🚀 Deployment
Backend: Render
Frontend: Vercel

Both deployments are pre-configured for CI pipelines using GitHub Actions.

## 🧪 Testing
### Backend:
pytest

### Frontend:
npm run test

## 🔐 Security

CORS properly configured

Rate limiting for public API routes

Production settings separated

HTTPS enforced in production

## 🗂 Issue Tracking

This project includes a full 50-issue development roadmap, covering:

Setup

Pages

API

Admin

Optimizations

CI/CD

Deployment

Import the CSV to generate all issues automatically.

## 🤝 Contributing

Pull requests are welcome!
Please open an issue before starting major work.

## 📜 License

MIT License — free to use, modify, and distribute.

## ⭐ Support

If you like this project, please leave a ⭐ star on GitHub —
It helps keep Animathics growing!
