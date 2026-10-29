# Match3 Sprite Solver

This repo is set up for a single-file static HTML app that runs on Vercel.

How to deploy on Vercel:
- push this repo to GitHub
- import it into Vercel
- choose the default static deployment settings
- Vercel will serve the root `index.html` automatically

What the app does:
- upload the full board screenshot
- upload a PNG crop of the goal item
- use OpenCV.js template matching to find the goal in the board
- test adjacent swaps
- return the best move as `from` and `to` cell coordinates

Notes:
- This is a browser-only HTML page.
- It does not require Node or TypeScript build tooling.
- It uses OpenCV.js loaded from the CDN at runtime.
- You can optionally add sprite PNGs into an `assets/` folder later, but the page works with uploaded PNGs directly.
