# ATSEA Scoreboard
## Overview
### Problem
- Who is affected?
  - Tournament organizers, streamers, and event hosts who need a clear and fast scoreboard during live matches.

- What is the issue?
  - Traditional scorekeeping can be slow, inconsistent, and difficult to display clearly in OBS or livestream setups. And ususally the streamer has to be both the scorekeeper and the scene changer for the live stream which is a lot to do among 
  the other possibilities the streamer might also be in charge of the tournament brackets.
  - After the tournament, the problem is that the streamer will always need to manually write and type out the details of the stream. It is manually tiring especially if the tournament takes a very long time and may even take hours to do.

### Outcome
- What was achieved?
  - A web-based scoreboard system that lets users update match information, scores, rounds, and tournament timing in real time.
  - The app includes a live overlay view that can be used with OBS and a WebSocket server for instant updates.
  - It includes a section where you can track and record matches details live on the website so that you won't have any trouble with the youtube description.

- Measurable results (if any)
  - Fast score updates during matches.
  - Persistent match recording history.
  - A tournament timer for event flow tracking.
  - An OBS-friendly overlay package for streaming use.

---

## Demo
- How does the solution work from the user’s perspective?
  1. Open the app and enter match details such as event host, game title, round, and players.
  2. Update scores and match state from the control interface.
  3. use either the link or download the zip files to use for your obs studio.
  4. Start the tournament timer and save match recordings for later review.

- Provide screenshots, GIFs or demo video.
  - Add screenshots or a short demo video here once available.

---

## Technology Stack
### Frontend components
- React with TypeScript
- Vite for development and build tooling
- CSS for styling the scoreboard UI and overlay
- Local storage for saving match state and recordings

### Backend components
- Node.js with Express
- WebSocket server for real-time communication
- TypeScript for server-side logic
- OBS-compatible HTML overlay output

---

## Installation
Ensure you are at the 'frontend' folder then:
1. Install dependencies:
   ```bash
   npm install
   ```

2. Start the development server in one terminal:
   ```bash
   npm run dev
   ```

3. Start the WebSocket server in a second terminal:
   ```bash
   npm run server
   ```

4. Open the local Vite URL in your browser. If prompted, press "o" in the Vite terminal to open it automatically.

---

## Usage
- using obs, create a new source in any scene you choose, and then create a browser source section. Inside it, choose the option for local file and then choose the index html from the zip.
- You can also choose to use the overlay link in the website instead.
- Use the scoreboard interface to enter or update match details.
- Adjust player names, scores, rounds, and game information as the match progresses.
- Click on save to store the details and update during or before matches.
- Start the tournament timer for event flow tracking.
- Review stored match recordings and update their timings accordingly to match the video you are about to upload on youtube.

---

## Project Structure
- src/ - main React application components, hooks, styles, and types
- src/components/ - scoreboard UI and overlay components
- src/hooks/ - custom hooks for WebSocket communication
- src/types/ - TypeScript type definitions for scoreboard, OBS, and recordings
- server/ - Node.js and WebSocket server implementation
- public/OBS_html_file/ - OBS overlay HTML package and assets
- docs/ai-dev/ - notes and documentation about the AI-assisted development workflow






































<!-- # React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Oxc](https://oxc.rs)
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/)

## React Compiler

The React Compiler is enabled on this template. See [this documentation](https://react.dev/learn/react-compiler) for more information.

Note: This will impact Vite dev & build performances.

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type-aware lint rules:

```js
export default defineConfig([
  globalIgnores(['dist']),
  {
    files: ['**/*.{ts,tsx}'],
    extends: [
      // Other configs...

      // Remove tseslint.configs.recommended and replace with this
      tseslint.configs.recommendedTypeChecked,
      // Alternatively, use this for stricter rules
      tseslint.configs.strictTypeChecked,
      // Optionally, add this for stylistic rules
      tseslint.configs.stylisticTypeChecked,

      // Other configs...
    ],
    languageOptions: {
      parserOptions: {
        project: ['./tsconfig.node.json', './tsconfig.app.json'],
        tsconfigRootDir: import.meta.dirname,
      },
      // other options...
    },
  },
])
```

You can also install [eslint-plugin-react-x](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-x) and [eslint-plugin-react-dom](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-dom) for React-specific lint rules:

```js
// eslint.config.js
import reactX from 'eslint-plugin-react-x'
import reactDom from 'eslint-plugin-react-dom'

export default defineConfig([
  globalIgnores(['dist']),
  {
    files: ['**/*.{ts,tsx}'],
    extends: [
      // Other configs...
      // Enable lint rules for React
      reactX.configs['recommended-typescript'],
      // Enable lint rules for React DOM
      reactDom.configs.recommended,
    ],
    languageOptions: {
      parserOptions: {
        project: ['./tsconfig.node.json', './tsconfig.app.json'],
        tsconfigRootDir: import.meta.dirname,
      },
      // other options...
    },
  },
])
``` -->
