# Tickett

A full-stack monorepo application using Turborepo to manage frontend and backend projects.

## Repository Structure

This is a **Turborepo monorepo** that contains both frontend and backend projects:

```
tickett/
├── apps/
│   ├── frontend/      # Next.js frontend application
│   └── backend/       # NestJS backend application
├── packages/          # Shared packages (optional)
├── package.json       # Root package.json with Turborepo
├── turbo.json         # Turborepo configuration
└── .gitignore         # Root-level gitignore
```

## Tech Stack

- **Monorepo Tool**: Turborepo
- **Frontend**: Next.js 16
- **Backend**: NestJS 11
- **Package Manager**: npm workspaces

## Getting Started

### Install Dependencies

From the root directory:

```bash
npm install
```

This will install all dependencies for both frontend and backend using npm workspaces.

### Development

Run all apps in development mode:

```bash
npm run dev
```

Or run specific apps:

```bash
# Frontend only
npm run dev --filter=@tickett/frontend

# Backend only
npm run dev --filter=@tickett/backend
```

### Build

Build all apps:

```bash
npm run build
```

### Other Commands

```bash
# Lint all apps
npm run lint

# Test all apps
npm run test

# Clean build artifacts
npm run clean
```

## Individual App Development

You can still work on individual apps directly:

```bash
# Frontend
cd apps/frontend
npm run dev

# Backend
cd apps/backend
npm run start:dev
```

## Benefits of Monorepo

- **Shared tooling**: Single configuration for linting, formatting, etc.
- **Faster builds**: Turborepo caches and parallelizes builds
- **Code sharing**: Easy to share code between frontend and backend
- **Atomic commits**: Changes across apps in single commits
- **Dependency management**: Single source of truth for dependencies
