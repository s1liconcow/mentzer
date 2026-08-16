# Mentzer - One Set

A dependency-free, mobile-first PWA for the two-day one-working-set-to-failure routine.

## Interaction model

The app is optimized for use between hard sets:

1. Start the workout - the previous/suggested load is already filled in.
2. Tap **Start set**.
3. At failure, tap the actual rep count.

That rep tap records weight + reps + set duration, advances to the next exercise, and starts the correct recovery timer. During recovery you can adjust the next load without another screen.

## Included routine

Workout A: leg extension -> leg press pre-exhaust, leg curl, low-incline DB press, high-cable pulldown, cable lateral raise, cable pressdown, calves.

Workout B: leg press, leg curl, hip thrust, weighted dip, low-cable row, DB overhead press, cable rear-delt fly, cable curl, calves.

Defaults: 15 sec pre-exhaust changeover, 2 min isolation recovery, 3 min compound recovery. All are editable.

## Features

- Automatically alternates A/B workouts
- Prefills last load and suggests an increment after hitting the top of the rep range
- One-tap failure logging
- Persistent rest timers that survive screen lock/app switching
- Local-only workout history
- Sound + vibration recovery alerts
- Installable/offline PWA
- No framework, account, backend, analytics, or network dependency after install

## Run

Serve the repository over HTTP, for example:

```bash
python3 -m http.server 4173
```

Then open `http://localhost:4173`.

For GitHub Pages, deploy the repository root. All paths are relative so it works at `/mentzer/`.
