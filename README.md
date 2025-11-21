# crypto-dashboard

A modern, responsive crypto dashboard built with Next.js, Tailwind CSS and React.

**Quick overview**: this repository contains a Next.js 15 app (React 19) with a collection
of UI components and utilities to build interactive crypto-related dashboards and charts.

**Tech stack**
- Next.js 15
- React 19
- Tailwind CSS
- TypeScript
- Recharts (charts)

## Features
- Responsive dashboard layout
- Reusable UI components (Radix + custom components)
- Charts and visualizations
- Theme support (dark/light)

## Prerequisites
- Node.js 18+ (LTS recommended)
- pnpm (recommended because this repo includes `pnpm-lock.yaml`), or `npm` / `yarn`

If you don't have `pnpm` installed, install it globally:

```powershell
npm install -g pnpm
```

## Quick start

1. Install dependencies

```powershell
pnpm install
# or: npm install
# or: yarn install
```

2. Run the development server

```powershell
pnpm dev
# or: npm run dev
```

Open http://localhost:3000 in your browser to view the app.

## Build for production

```powershell
pnpm build
pnpm start
# or: npm run build && npm run start
```

## Scripts
- `dev` - Run Next.js in development mode
- `build` - Build the production bundle
- `start` - Start the production server
- `lint` - Run Next.js linting

## Environment variables
This project does not include required environment variables in the repo. If the app
needs API keys or other secrets, create a `.env.local` file in `crypto-dashboard/` and add
any necessary `NEXT_PUBLIC_` environment variables or server-side variables used by the app.

Example `.env.local` (if needed):

```text
# NEXT_PUBLIC_API_URL=https://api.example.com
# NEXT_PUBLIC_ANALYTICS_KEY=your_key_here
```

## Project structure (top-level)
- `crypto-dashboard/` - Next.js application
	- `app/` - Next.js app directory (pages, layout, global styles)
	- `components/` - UI components used across the app
	- `public/` - static assets
	- `styles/` - global styles and Tailwind setup

## Contributing
- Open an issue or submit a pull request.
- Follow the existing code style and run linting before opening a PR:

```powershell
pnpm lint
```

## Troubleshooting
- If you run into dependency issues, try removing `node_modules` and reinstalling:

```powershell
rm -r node_modules
pnpm install
```

On Windows PowerShell replace `rm -r` with `Remove-Item -Recurse node_modules` if needed.

## License
See the `LICENSE` file in the repository root.

---
If you'd like, I can also:
- run the dev server for you now in a terminal, or
- add a short development checklist or example environment variables used by the dashboard.
