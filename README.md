# AWS Challenge Kanban Dashboard

This repository contains Phase 1 of a beginner-friendly 3-tier Kanban application:

- `frontend/` contains a static HTML, CSS, and JavaScript dashboard ready for Vercel.
- `backend/` contains a Python Flask API ready for local development and later deployment to EC2.
- `deploy/` contains example server files for Gunicorn and Nginx on EC2.
- `docs/` contains simple step-by-step guides for setup and deployment.

## Phase 1 features

- View tasks in `To Do`, `In Progress`, and `Done` columns
- Create new tasks
- Edit existing tasks
- Delete tasks
- Move tasks between columns with a dropdown
- Drag and drop tasks between columns
- Save tasks in a SQLite database

## Project structure

```text
frontend/   Static frontend files
backend/    Flask backend files
deploy/     EC2 deployment templates
docs/       Beginner-friendly guides
```

## Best starting points

- Local run: `docs/PHASE1_SETUP.md`
- EC2 walkthrough: `docs/EC2_DEPLOYMENT_STEP_BY_STEP.md`
- Architecture overview: `docs/ARCHITECTURE.md`
