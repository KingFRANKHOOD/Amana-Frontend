# Amana Frontend

This repository contains the Amana frontend application built with Next.js.
It is the user-facing interface for buyers, sellers, and mediators interacting with the Amana escrow protocol.

## Features

- Next.js 16 App Router
- React 19 UI components
- Tailwind CSS styling
- Playwright visual regression testing
- Jest unit/integration testing
- Stellar wallet integration via Freighter
- Privacy-first analytics instrumentation

## Getting Started

### Prerequisites

- Node.js 20+ / npm
- A `.env.local` file configured for the frontend environment

### Install dependencies

```bash
cd Amana-Frontend
npm install
```

### Environment

Copy the example env file and configure your runtime variables:

```bash
cp .env.example .env.local
```

### Run in development

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### Build

```bash
npm run build
```

### Start production server

```bash
npm run start
```

### Linting

```bash
npm run lint
```

### Tests

```bash
npm test
npm run test:coverage
npm run test:visual
```

### Visual regression tests

```bash
npm run test:visual
npm run test:visual:update
```

## Notes

- `app/` contains the Next.js application and page routing.
- `src/` contains shared components, hooks, and utilities.
- `public/` holds static assets and images.
- `playwright.config.ts` controls Playwright visual regression.

## Repository Scope

This frontend repo was extracted from the main `Amana/` monorepo and now serves as the dedicated UI repository for the Amana project.

If you are consuming the backend API, point the frontend environment configuration to the Amana Backend Service API endpoint.
