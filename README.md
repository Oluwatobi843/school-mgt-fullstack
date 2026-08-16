# School Management Dashboard

> A Next.js dashboard application for a school-management platform.

## Overview

School Management Dashboard is the frontend/dashboard component of a broader school-management system. The application provides a foundation for presenting school data and administrative workflows through a modern web interface.

This repository is currently focused on the dashboard/frontend layer. The dedicated backend API is maintained separately in the `school-management-backend` repository.

## Technology Stack

| Layer | Technology |
|---|---|
| Framework | Next.js 14 |
| UI | React 18 |
| Language | TypeScript 5 |
| Styling | Tailwind CSS |
| Database tooling | Prisma |
| Code quality | ESLint |

## Architecture

```text
Browser
   |
   v
Next.js Application
   |
   +--> Dashboard UI
   +--> Pages / App Router
   +--> Reusable React components
   +--> API/data integration
   |
   v
School Management Backend
   |
   v
PostgreSQL
```

The frontend is designed to consume backend services rather than placing core business logic directly in the browser.

## Project Structure

The application follows the Next.js App Router structure.

```text
school-mgt-fullstack/
├── app/                 # Next.js routes and application UI
├── components/          # Reusable UI components where applicable
├── public/              # Static assets
├── prisma/              # Prisma configuration/schema where applicable
├── package.json
├── tsconfig.json
└── tailwind.config.*
```

## Getting Started

### Prerequisites

- Node.js 18+
- npm, yarn, pnpm or Bun
- Access to the school-management backend for API-backed workflows

### Clone

```bash
git clone https://github.com/Oluwatobi843/school-mgt-fullstack.git
cd school-mgt-fullstack
```

### Install dependencies

```bash
npm install
```

### Run development server

```bash
npm run dev
```

Open `http://localhost:3000` in your browser.

## Production build

```bash
npm run build
npm run start
```

## Linting

```bash
npm run lint
```

## Backend integration

The frontend should be documented and configured around the API exposed by the companion backend repository:

**School Management Backend**

https://github.com/Oluwatobi843/school-management-backend

When connecting the applications, keep API URLs and credentials in environment variables rather than hard-coding them in client code.

## Development goals

The dashboard is intended to evolve into a complete school-management interface supporting areas such as:

- Authentication
- Student management
- Class management
- Attendance
- Academic records
- Administrative workflows
- User and role management

Only features that are implemented in the current codebase should be presented as production functionality.

## Engineering Focus

This repository demonstrates:

- Next.js application development
- React component architecture
- TypeScript
- Responsive dashboard development
- Tailwind CSS
- Frontend/backend separation
- API integration foundations
- Prisma tooling

## Roadmap

Potential improvements include:

- Connect all dashboard workflows to the production backend API
- Add authenticated route protection
- Implement student/class/attendance views
- Add loading, error and empty states
- Add form validation
- Add frontend testing
- Add role-specific dashboards
- Add production deployment configuration

## Related Project

For the backend API and database-focused implementation, see:

https://github.com/Oluwatobi843/school-management-backend

## Author

**Oluwatobi843**

GitHub: https://github.com/Oluwatobi843

## License

See the repository license for applicable terms.
