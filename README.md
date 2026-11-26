# Pixel Racers
Local: `npm install` then `npm run dev` (server :8080, web :5173). Tests: `npm test`.
Controls: Arrows/WASD (X also brakes), Space boost, R reset.
## Render (server)
New Blueprint from this repo (uses render.yaml). Set `ALLOWED_ORIGINS` to your Vercel URL. Free tier sleeps; the client shows "Waking up the server..." and retries with backoff.
## Vercel (web)
Import repo, set env `VITE_SERVER_URL=https://YOUR-SERVICE.onrender.com`. vercel.json handles build/output.
## Tuning
All physics constants are in `packages/shared/src/index.ts` (`CFG`).
