# Desk Racer

A miniature desk-coaster time-trial racer for the browser, built with Three.js and Rapier physics.
Race 3 laps around a 1:87-scale coaster that winds across a cluttered desk, with a chase cam, cockpit cam,
full-desk view and drone view, synthesized engine audio and touch controls for phones.

## Controls
| Key | Action |
|---|---|
| W / Up | Accelerate |
| S / Down | Brake |
| A, D / Left, Right | Steer |
| 1 - 4 | Chase, cockpit, full-desk and drone cameras |
| M | Mute / unmute |
| Enter | Start time trial |

On touch devices, on-screen buttons appear automatically.

## Run locally
```
npm install
npm run dev        # http://localhost:3000
```

## Build and deploy
```
npm run build      # outputs ./dist
npm run preview    # serve the production build
```
`dist/` is fully static: upload it to any static host (Netlify, GitHub Pages, itch.io, S3...).

## 3D models
The four optional `.glb` models (desk props, kart, room, track) are downloaded from gstatic at build
time and also fetched at runtime if online. If they are unavailable the game automatically uses its
built-in procedural models, so it is playable fully offline.
