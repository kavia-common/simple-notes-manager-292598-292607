# Notes Frontend (Astro)

A simple local-only notes application with a modern "Ocean Professional" UI. Create, search, edit, and delete notes directly in your browser using localStorage. No backend required.

## Features

- Responsive layout: sidebar list + editor on desktop, stacked on mobile
- Create, edit, and delete notes (with confirmation)
- Autosave for title and body with debounce to reduce writes
- Search/filter notes by title or body
- Sort notes by Last Updated (desc) or Title (A–Z)
- Persistent storage via localStorage (`notes.v1`)
- Accessible components and keyboard navigation for the list
- Smooth transitions, subtle shadows, and a clean professional theme
- Optional light/dark toggle

## Getting Started

From this `notes_frontend` directory:

- Install dependencies
  npm install

- Start the dev server
  npm run dev
It should be available at http://localhost:3000 (or the configured port in astro.config.mjs).

- Build for production
  npm run build

- Preview the build locally
  npm run preview

## Environment Variables

This app does not require a backend. If public environment variables exist (e.g., PUBLIC_API_BASE, PUBLIC_FRONTEND_URL), they are not used by default.

## Data Persistence

Notes are stored in your browser's localStorage under the key `notes.v1`. Clearing site data or using a different browser/device will result in an empty set of notes.

## Keyboard Tips

- In the notes list, press Enter or Space to select the focused note.

## License

MIT
