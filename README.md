# NumeriX — Interactive Numerical Methods Calculator

> Bahria University Karachi · BSE-6C · Numerical Analysis Project

A full-stack interactive web platform implementing 13 labs of numerical methods with real-time computation, iteration tables, and live charts.

---

## 🔥 Name
**NumeriX** — *Numer* (Numerical) + *X* (unknown, solving for x)

---

## 📦 Project Structure

```
numerix/
├── frontend/     ← React + Tailwind CSS (deploy to Vercel)
└── backend/      ← Python FastAPI (deploy to Vercel / Railway)
```

---

## 🧩 Modules Covered

| Module | Methods | Labs |
|--------|---------|------|
| Error Analyzer | Absolute, Relative, Round-off, Truncation | Lab 2 |
| Root Finder | Bisection, False Position, Newton-Raphson, Fixed-Point | Labs 4–5 |
| Interpolator | Newton Forward/Backward, Divided Difference, Lagrange | Labs 6–7 |
| Differentiator | Forward & Backward Finite Differences (1st & 2nd order) | Lab 8 |
| Integrator | Trapezoidal, Simpson's 1/3, Simpson's 3/8, Unequal Segments | Labs 9–10 |
| ODE Solver | Euler, Improved Euler, Runge-Kutta 4th Order | Labs 11–12 |
| Linear Systems | LU Decomposition (Doolittle & Crout) | Lab 13 |

---

## 🚀 Local Setup

### Backend (FastAPI)
```bash
cd backend
pip install -r requirements.txt
uvicorn main:app --reload --port 8000
```

### Frontend (React)
```bash
cd frontend
cp .env.example .env          # set REACT_APP_API_URL=http://localhost:8000
npm install
npm start
```

Open http://localhost:3000

---

## ☁️ Deployment on Vercel

### Step 1 — Deploy Backend
1. Go to [vercel.com](https://vercel.com) → New Project → import `backend/` folder
2. Framework: **Other**
3. Root Directory: `backend`
4. Deploy → copy the URL (e.g. `https://numerix-api.vercel.app`)

### Step 2 — Deploy Frontend
1. New Project → import `frontend/` folder
2. Framework: **Create React App**
3. Root Directory: `frontend`
4. Add Environment Variable:
   - `REACT_APP_API_URL` = `https://numerix-api.vercel.app` (your backend URL)
5. Deploy ✅

> **Alternative Backend**: Deploy backend to [Railway](https://railway.app) for persistent FastAPI hosting (recommended over Vercel for Python).

---

## 🛠 Tech Stack

| Layer | Tech |
|-------|------|
| Frontend | React 18, Tailwind CSS, Recharts, React Router |
| Backend | Python, FastAPI, Uvicorn, Pydantic |
| Deployment | Vercel (frontend + backend) |
| Fonts | Space Grotesk, JetBrains Mono, Inter |

---

## 📐 Design System

- **Color**: Dark obsidian background `#080B14` with neon cyan `#00F5FF` accents
- **Type**: Space Grotesk (display) + JetBrains Mono (data/code) + Inter (body)
- **Signature**: Glowing neon-on-dark aesthetic with glass-morphism cards

---

*Made for BSE-6C Numerical Analysis Final Project — Bahria University Karachi Campus*
