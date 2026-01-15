# Tickett

A full-stack application with separate frontend and backend projects, all tracked in a single git repository.

## Repository Structure

This is a **single git repository** that contains both frontend and backend projects:

```
tickett/
├── frontend/          # Next.js frontend application
├── backend/           # NestJS backend application
└── .gitignore         # Root-level gitignore for both projects
```

## Projects

### Frontend
- **Location**: `frontend/`
- **Framework**: Next.js
- **Setup**: See [frontend/README.md](./frontend/README.md)

### Backend
- **Location**: `backend/`
- **Framework**: NestJS
- **Setup**: See [backend/README.md](./backend/README.md)

## Development

Each project has its own dependencies and can be run independently:

```bash
# Frontend
cd frontend
npm install
npm run dev

# Backend
cd backend
npm install
npm run start:dev
```

## Git Repository

This is a **single git repository** tracking all changes in both frontend and backend directories. All commits are made from the root directory.
