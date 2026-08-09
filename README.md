# Chaudhary's Carpet | Production Frontend

This repository houses the production-ready React + Vite frontend for Chaudhary's Carpet, strictly optimized for performance, robust state management, secure validation, and SEO according to an absolute visual lock rule constraint framework.

## Setup & Local Development

1. **Install dependencies**:
   ```bash
   npm install
   ```
2. **Environment Handling**:
   Copy `.env.example` to `.env` and fill in the required values.
   ```bash
   cp .env.example .env
   ```
3. **Start the Dev Server**:
   ```bash
   npm run dev
   ```

## Production Build & Deployment

The application is bundled using Vite with code-splitting logic tailored to separate dependencies effectively.

1. **Create the Build**:
   ```bash
   npm run build
   ```
   *This outputs to the `dist/` directory.*

2. **Preview the Build**:
   ```bash
   npm run preview
   ```

### Deployment

Deploy the `dist/` output to any static hosting provider (Vercel, Netlify, AWS S3 + CloudFront). Note: as this is a React Router SPA, ensure your staging or hosting server rules are configured to redirect all fallback routes to `index.html`.

## Code Standard Enforcement

- **ESLint** configuration is managed via `.eslintrc.cjs`. Run `npx eslint "src/**/*.{js,jsx}"` if configured in your scripts.
- **Prettier** is used for strict formatting checks. See `.prettierrc`.
- Form validation utilizes `react-hook-form` coupled with `yup` resolving schemas safely. 

## Architecture Note

*Strict visual locks govern this repository.* Do not modify base Tailwind utility sets, JSX layouts, margins, padding, or structural dom elements unless accompanied by a complete visual audit. Components reside in `src/components`, layouts span throughout routing config `src/App.jsx`, hooks in `src/hooks`, API wrappers under `src/services`, and Redux slices across `src/store`.

Made with ❤️ for Chaudhary's Carpet · Est. 1987
