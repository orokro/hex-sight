# Hex Sight Reading 🎨

Learn to *sight-read hex colors* with **Hex‑chan**, your anime tutor for color theory and code literacy!  
This project gamifies RGB hex notation into a series of mini‑games and lessons that train your eye to read and understand colors directly from hex codes.

---

## 🚀 Features

- 🧠 **Progressive Learning**
  - Start with 4‑bit single‑channel (Red, Green, Blue)
  - Learn mixing pairs (RG, GB, RB)
  - Advance to full 8‑bit RGB sight reading

- 🎮 **Mini Games**
  - **Guessing Game** — estimate color intensity from hex
  - **Coloring Book** — fill SVGs by hex code accuracy
  - **Matching** — match hex codes to color swatches
  - **Bartender** — mix RGB “drinks” to match requested hex values

- 💬 **Hex‑chan Avatar**
  - Animated dialog & reactions to your progress
  - State‑based mouth/eye/pose controller

- 🧩 **Modern Vue Stack**
  - Vue 3 (Composition API + TypeScript)
  - Pinia for state management
  - Vite for build/dev
  - Vitest + Vue Test Utils + Playwright for testing

---

## 🏗️ Project Setup

### Prerequisites
- Node.js ≥ 20
- npm ≥ 9

### Create the Project
```bash
npm create vite@latest hex-sight -- --template vue-ts
cd hex-sight
npm install
```

### Add Dependencies
```bash
npm install pinia vue-router @vueuse/core
npm install -D vitest @vue/test-utils @testing-library/vue playwright eslint prettier
npx playwright install
```

---

## 🧠 Development Scripts

| Command | Description |
|----------|-------------|
| `npm run dev` | Start the dev server |
| `npm run build` | Build for production |
| `npm run preview` | Preview production build |
| `npm run test` | Run unit/component tests |
| `npx playwright test` | Run end‑to‑end tests |

---

## 🧩 Architecture Overview

```
src/
├─ app/              # main.ts + router
├─ color-engine/     # pure TypeScript color logic
├─ components/       # UI + game elements
├─ games/            # Guessing, Coloring, Matching, Bartender
├─ stores/           # Pinia stores
├─ types/            # shared type definitions
└─ tests/            # Vitest & Playwright tests
```

---

## 🧪 Testing Stack

- **Unit**: Vitest
- **Component**: Vue Test Utils + Testing Library
- **E2E**: Playwright

Start with pure TypeScript tests in `color-engine`, then move up to component and E2E layers.

---

## 🗺️ Roadmap

1. Core color engine (conversions, scoring, lessons)
2. Guessing Game (4‑bit → 8‑bit)
3. Coloring Book (SVG cells)
4. Matching / Bartender minigames
5. Hex‑chan puppet + dialog system
6. Roadmap screen & progression tracking
7. Accessibility & polish

---

## 🧠 Learning Goals

This project doubles as a playground for mastering:

- TypeScript with Vue 3 Composition API
- Pinia for state management
- Unit, component, and E2E testing
- Modular game architecture in a SPA
- CSS/SVG animation techniques

---

## 🖤 Credits

Created by **geem4**  
Concept & design: *Hex‑chan — your color code sensei*

---

### License
MIT © geem4
