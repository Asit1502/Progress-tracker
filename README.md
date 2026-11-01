# Data Engineering Study Tracker

A responsive, browser-based 12-week Data Engineering preparation tracker, built with React and Vite.

## Features

- Complete Monday–Friday plan for 12 weeks (60 days, 240 time-block checkboxes)
- Daily 8–10 PM study timetable: 45 minutes Udemy, 25 minutes reading, 40 minutes practice, 10 minutes review
- Detailed reading and coding assignments for each day
- Course progress slider and optional Udemy link
- Project milestone checklist and project name
- Notes for each study day
- Dashboard with progress metrics
- Local automatic persistence and JSON export/import backup

## Run locally

Requires Node.js 18+.

```bash
npm install
npm run dev
```

## Deploy to Vercel

1. Create a new GitHub repository and upload this project's files (including `package.json`, `index.html`, `src.jsx`, and `style.css`).
2. Open https://vercel.com/new and import the GitHub repository.
3. Select **Vite** if prompted. Build command: `npm run build`. Output directory: `dist`.
4. Click **Deploy**. Vercel will give you a public URL.

Alternatively, install the Vercel CLI and run `npx vercel` from the project folder.

## Deploy to Netlify

1. Run `npm install && npm run build`.
2. Upload the `dist` directory at https://app.netlify.com/drop .

## Data persistence

Progress is stored in your browser's `localStorage`, not on a server. It does not automatically sync across devices. Use **Export backup** to save a JSON file and **Import** to restore on another browser/device. Clearing browser storage removes progress unless you have a backup.

## Customize

Change the `raw` array in `src.jsx` to update weekly topics and tasks. Change `slots` to adjust the daily timetable.
