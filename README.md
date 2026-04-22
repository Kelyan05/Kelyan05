# Kelyan Djomo

Final-year CS student at the University of Westminster, graduating 2026. I build full-stack applications with a focus on backend architecture, API design, and systems that are easy to reason about. Currently open to graduate software engineering roles in London.

📍 London, UK · darrelkelyan@outlook.com · [LinkedIn](https://linkedin.com/in/your-link)

---

## Projects

### [SignalFM](https://github.com/Kelyan05/SignalFM) · [Live demo ↗](https://signalfm-site.onrender.com)

A full-stack music streaming platform with a real-time, event-driven recommendation engine. Built as my Computer Science FYP.

The recommendation engine captures every play, skip, and like as a weighted engagement signal — play: +1, skip: −2, like: +3 — grounded in the implicit feedback model by Hu, Koren & Volinsky (2008). Each interaction triggers a server-side cache invalidation so the next recommendation request reflects fresh behavioural data immediately.

`React 18` `Node.js` `Express` `Firebase Firestore` `Spotify SDK` `Render`

- Domain-driven custom hook architecture (`useTrackEvents`, `useRecommendations`, `useSpotifyPlayer`) — largest component reduced from ~200 lines of mixed logic to under 50 lines of pure presentation
- BFF OAuth 2.0 flow: backend exchanges the Spotify authorisation code, tokens never touch the client
- Global playback state via React Context (`PlayerContext`, `LikedTracksProvider`) — single source of truth across all components
- 63 functional test cases across 9 feature areas; 98% pass rate on first submission

---

### [HyJacked](https://github.com/SleepyXm/hyjacked) (Currently working on)

A real-time paper trading platform built with a university peer, combining a Next.js frontend with a Python/FastAPI backend.

`Next.js` `FastAPI` `Python` `WebSockets`

- Multi-interval stock data API supporting 8 timeframes via both REST and WebSocket endpoints
- Real-time candlestick and line charts with live WebSocket data feeds and automatic candle updates
- Paper trading engine with live P&L tracking, spread calculation, and price-line visualisation
- Asset search with intraday chart previews for discovered symbols

---

## Tech

**Languages:** JavaScript · TypeScript · Python · HTML/CSS  
**Frontend:** React 18 · Next.js  
**Backend:** Node.js · Express · FastAPI · REST · WebSockets  
**Data & infra:** Firebase Firestore · Docker · Git · Postman · Render
