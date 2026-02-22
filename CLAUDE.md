# CLAUDE.md

## Project Overview

FB Corp Flywheel is an interactive single-page dashboard that visualizes the 2026 Integrated Growth Flywheel for FB Corp. It presents a circular flywheel UI with five interconnected business stages (Execution, Media, Skool, Capital, Scale), each with detailed inputs, outputs, and tech optimizations. The flywheel auto-rotates through stages and allows manual selection.

## Tech Stack

- **Framework**: React 18 (JSX, functional components with hooks)
- **Build Tool**: Vite 4
- **Styling**: Tailwind CSS 3 (utility classes, dark theme with `slate-950` base)
- **Icons**: lucide-react
- **Language**: JavaScript (no TypeScript)

## Project Structure

```
fb-corp-flywheel/
├── index.html          # Vite entry point HTML
├── package.json        # Dependencies and scripts
├── vite.config.js      # Vite config (React plugin only)
├── src/
│   ├── App.jsx         # Entire application (single-file SPA)
│   └── Appjsx          # Legacy/alternate HTML entry (unused by Vite)
└── README.md
```

The application is entirely contained in `src/App.jsx` — there is no routing, no state management library, and no separate component files. All components (`FlywheelSegment`, `App`) and data (`FLYWHEEL_DATA`) live in this single file.

## Development Commands

```bash
npm install        # Install dependencies (must run first)
npm run dev        # Start Vite dev server with HMR
npm run build      # Production build to dist/
npm run preview    # Preview production build locally
```

There is no test framework, linter, or formatter configured.

## Architecture & Key Patterns

### State Management
- All state is local React state via `useState` / `useEffect` hooks
- `activeSegment` — currently displayed flywheel segment
- `isRotating` — controls the 5-second auto-rotation interval
- `copied` — transient UI feedback for the share button

### Component Structure
- **`App`** — root component; header, flywheel visual, detail panel, footer stats
- **`FlywheelSegment`** — positioned via CSS transforms around a circular layout (`rotate + translateY + counter-rotate`)

### Data Model
`FLYWHEEL_DATA` is a static array of 5 segment objects, each containing:
- `id`, `title`, `subtitle`, `description` — display text
- `icon` — JSX lucide-react icon element
- `color`, `bg`, `border` — Tailwind class strings for theming
- `inputs`, `outputs`, `tech` — string arrays for detail panel lists

### Styling Conventions
- Tailwind utility classes exclusively (no custom CSS files)
- Dark theme: `slate-950` background, `slate-100` text
- Each flywheel segment has a distinct color palette (blue, purple, orange, emerald, red)
- Custom keyframe animations defined via inline `<style dangerouslySetInnerHTML>` for `spin-slow` and `reverse-spin`

## Key Conventions

- **Single-file architecture**: Keep all components in `src/App.jsx` unless the app grows significantly
- **No TypeScript**: The project uses plain JSX; do not introduce `.tsx` files
- **Tailwind-only styling**: Do not add CSS modules or styled-components; use Tailwind utility classes
- **Static data**: `FLYWHEEL_DATA` is hardcoded at the top of `App.jsx`; there are no API calls or backend
- **No tests**: There is no test infrastructure; if adding tests, use Vitest (Vite-native)
- **JSX icons**: Icons are stored as JSX elements directly in the data array, not as string references

## Notes

- `src/Appjsx` is a legacy HTML file from an earlier iteration. It is not used by the Vite build and can be ignored or removed.
- The `index.html` at the project root is the Vite entry point and includes a `<script type="module" src="/src/App.jsx">` tag — this is the standard Vite setup.
- No `.gitignore` is present; `node_modules/` and `dist/` are not tracked only because `npm install` has not been run in the committed state.
