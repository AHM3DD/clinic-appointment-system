# Project Phases — Clinic Appointment System

## Phase 0 — Environment & Repo (completed)
Goal
- Prepare developer environment and initialize repository.

What I completed
- OS: Windows 11
- Python venv: backend/.venv (activated during work)
- Git: repo initialized, branch `main`
- Remote: origin -> https://github.com/AHM3DD/clinic-appointment-system.git
- Files added: `.gitignore`, `.env.example`, `README.md` (project info), `backend/`, `frontend/`
- Confirmed working tree is clean and pushed initial commit

How to replicate (commands run)
- Create venv (if needed): `python -m venv backend\.venv`
- Activate venv (PowerShell): `backend\.venv\Scripts\Activate.ps1`
- Git init & push:
  - `git add .`
  - `git commit -m "chore: initial project scaffold"`
  - `gh repo create AHM3DD/clinic-appointment-system --public --source=. --remote=origin --push`

Notes / next
- Keep `.env` out of repo and add secrets in GitHub settings
- Next step: Start Phase 1 — scaffold FastAPI backend. To begin, say "Start Phase 1".

## Phase 1 — Backend skeleton (FastAPI)
- Create `backend/main.py`, `backend/requirements.txt`
- Add simple /health and /appointments endpoints
- Configure CORS for React dev

## Phase 2 — Database (Postgres + ORM)
- Add SQLModel/SQLAlchemy models, migrations, and DATABASE_URL config

## Phase 3 — RAG intent layer (ChromaDB)
- Build embedding + small vector store to map symptom text → specialty

## Phase 4 — Telegram bot + ngrok
- Implement webhook bot (python-telegram-bot), configure ngrok, connect to backend intent API

## Phase 5 — Frontend (React)
- Scaffold React app: Dashboard, AppointmentForm, AppointmentList

## Phase 6 — Tests & docs
- Unit tests, CI, optional docker-compose, deployment notes