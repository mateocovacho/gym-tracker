# Gym Tracker

![Dashboard Screenshot](https://github.com/mateocovacho/gym-tracker/blob/main/resources/dashboard.png?raw=true)

Granular gym tracking with muscle-level analytics. Know exactly which muscles are ready to work.

## Features

- **80+ Exercises** with detailed muscle targeting
- **Muscle Recovery Tracking** - see which groups are recovered
- **Smart Recommendations** based on workout history
- **FitNotes Import** - migrate your existing data
- **Responsive Dark UI** optimized for gym use

## Quick Start

### Docker
```bash
docker-compose up
```
App runs at `http://localhost:3005`

### Local
```bash
cd app
npm install
npm run dev
```

## Import from FitNotes

1. Export your FitNotes data as CSV
2. Place as `exportedFitNotes.csv` in project root
3. Run: `node import_local.js`

Or upload via the Settings UI.

## Tech Stack

- **Frontend**: Svelte 4 + Vite
- **Backend**: Express.js
- **Database**: SQLite
- **Icons**: Lucide Svelte

## Muscle Groups Tracked

Chest, Back, Shoulders, Arms (bi/triceps), Legs, Core, Neck - 21+ muscles total.

## License

MIT
