# KindPulse — The Daily Kindness Hub

KindPulse is a responsive, interactive kindness platform that helps people discover small daily acts, record progress, share good deeds, and celebrate community impact.

## Features

- 16 navigable page views across personal progress, challenge discovery, community, events, achievements, impact, profile, and settings.
- Daily kindness prompt generator and once-per-day completion tracking.
- Community wall with story submission, likes, category filters, and search.
- Personal dashboard, seven-day streak view, monthly kindness calendar, and journal.
- Saved challenges, group membership and event-interest interactions, achievements, and a sample leaderboard.
- Responsive desktop and mobile layouts.
- Three-line hamburger menu with a left sliding drawer, close button, backdrop dismissal, Escape-key support, and automatic close after navigation.
- Browser-local persistence through `localStorage`.

## Tech stack

- React 19 and TypeScript
- Vite 6
- Lucide React icons
- CSS for the theme, components, and responsive layouts

## Run locally

Requirements: Node.js 18 or newer and npm.

```bash
npm install
npm run dev
```

Vite prints the local development URL in the terminal.

## Production build

```bash
npm run build
npm run preview
```

The production bundle is generated in `dist/`.

## Deployment

This is a frontend-only Vite application and can be deployed to Vercel, Netlify, or another static hosting provider.

For Vercel:
- Framework preset: Vite
- Build command: `npm run build`
- Output directory: `dist`
- Install command: `npm install`

No environment variables are required for the current demo.

## Demo data and privacy

The app runs without a hosted backend. User-created stories, likes, journal entries, saved challenges, and kindness progress are stored in the current browser using local storage. Demo community members, leaderboard scores, events, and aggregate impact figures are illustrative sample content. Data does not synchronize across devices or browsers. Do not enter sensitive personal information.

Use **Settings → Data & privacy → Reset local demo data** to clear local app state.

## Project structure

```text
index.html              Vite HTML entry point
src/
  App.tsx               App pages, navigation, state, and interactions
  index.css             Theme, component styles, and responsive layouts
  main.tsx              React application entry point
tests/
  tests.json            Manual and QA test scenarios
package.json            Dependencies and npm scripts
postcss.config.js       PostCSS configuration
tailwind.config.js      Tailwind content configuration
tsconfig.json           TypeScript compiler settings
vite.config.ts          Vite and React plugin configuration
```

## QA scenarios

See [tests/tests.json](tests/tests.json) for documented functional and responsive scenarios covering navigation, challenge completion, community interactions, local persistence, profile settings, and form validation.
