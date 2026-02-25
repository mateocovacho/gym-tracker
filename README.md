# Gym Tracker

A granular gym tracking application built with Svelte, Vite, Express, and SQLite. Track your workouts with detailed muscle-level analytics and intelligent recommendations.

## Features

- **Comprehensive Exercise Library**: 80+ exercises with detailed muscle targeting
- **Granular Tracking**: Track sets, reps, and weight for each exercise
- **Muscle Recovery Analysis**: See which muscle groups are ready for work
- **Smart Recommendations**: Get workout suggestions based on muscle recovery
- **FitNotes Import**: Import your existing workout history from FitNotes
- **Responsive Design**: Blueprint-inspired dark UI optimized for desktop and mobile
- **Docker Support**: Easy deployment with Docker Compose

## Tech Stack

- **Frontend**: Svelte 4 + Vite
- **Backend**: Express.js
- **Database**: SQLite (better-sqlite3)
- **Icons**: Lucide Svelte
- **Styling**: Custom CSS with Blueprint-inspired design

## Quick Start

### With Docker

```bash
docker-compose up
```

The app will be available at `http://localhost:3005`

### Local Development

```bash
cd app
npm install
npm run dev
```

Backend runs on port 3000, frontend dev server on port 5173.

## Data Import

To import your FitNotes data:

1. Export your data from FitNotes as CSV
2. Place it in the project root as `exportedFitNotes.csv`
3. Run: `node import_local.js`

Or use the web interface in Settings to upload your CSV.

## Exercise Mapping

The app includes intelligent exercise name mapping from common FitNotes names to the app's exercise database. See `list_exercises.js` for the full mapping configuration.

## Muscle Groups Tracked

- **Chest**: Upper chest, mid chest, lower chest
- **Back**: Traps, lats, mid back, lower back
- **Shoulders**: Front delts, side delts, rear delts
- **Arms**: Biceps (long/short head), triceps (long/lateral/medial head), forearms
- **Legs**: Quads, hamstrings, glutes, calves
- **Other**: Abs, neck

## License

MIT
