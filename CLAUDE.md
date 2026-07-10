# Super Calculator

## Project overview
A beginner-friendly Angular 19 calculator built for teaching purposes. It's a
teaching scaffold: students implement missing methods and unit tests following
step-by-step instructions in `requirements.md`.

## Tech stack
- Angular 19 (standalone components, no NgModules)
- TypeScript ~5.7
- Karma + Jasmine for unit tests

## How to run
- Install: `npm install`
- Dev server: `npm start` → http://localhost:4200
- Tests: `npm test`
- Production build: `npm run build` (output in `dist/`)

## Project structure
- `src/app/app.component.ts` — all calculator state and logic (digit entry,
  operators, clear, sign toggle, percent, theme toggle)
- `src/app/app.component.html` — template, binds buttons to component methods
- `src/app/app.component.css` — scoped styles, including dark/light theme rules
- `src/app/app.component.spec.ts` — unit tests (Karma + Jasmine)
- `src/app/app.config.ts` — application bootstrap configuration
- `src/main.ts` — app entry point
- `karma.conf.js` — test runner configuration
- `requirements.md` — the exercise instructions this project was built around

## Exercises
This repo was built around three student exercises defined in `requirements.md`,
all now implemented:
- **Part 1** — `pressToggleSign()`, `pressPercent()`, and `toggleTheme()` (+ light
  mode CSS) in `app.component.ts`/`app.component.css`.
- **Part 2** — the 12 previously-`pending()` unit tests in `app.component.spec.ts`.
- **Part 3** — this file.

If similar methods appear empty/TODO again in the future (e.g. on a reset
branch), treat them as intentional teaching placeholders, not bugs.

## Coding conventions
- JSDoc-style comments explain *why*, not what — the code favors clear names
  over comments.
- Section dividers use `// ─── Section ───` comments to group related methods.
- Methods are named by the button they handle: `pressDigit`, `pressOperator`,
  `pressEquals`, `pressClear`, `pressToggleSign`, `pressPercent`, `toggleTheme`.
- Internal-only logic (e.g. `calculate()`) is marked `private`.
- 2-space indentation, single quotes, semicolons — standard Angular CLI defaults.
