# Curated Art Showcase (Static)

A single-file static website where multiple artists can upload their artwork (stored in the browser), curators can approve submissions, visitors can browse a gallery with zoom/pan, and anyone can preview art on their own wall by uploading a room photo. No login. No payments.

## Features
- Multiple artist uploads (saved to localStorage)
- Curator approval flow (pending -> approve/remove)
- Gallery with search & artist filter
- Zoom & pan image viewer
- Room/Wall visualization: upload a wall photo, overlay chosen artwork, drag/scale/rotate
- Display-only: no checkout, no buyer accounts

## Quick Start
Just open `index.html` in a modern browser.
(If images don’t load due to file URL policies, run a tiny local server: `python3 -m http.server` and visit http://localhost:8000)

## Notes
- This demo stores data in the browser’s localStorage. In production, connect real storage (S3, Firebase, Supabase, etc.) and a simple admin endpoint for curation.
- Mobile camera capture is enabled on file inputs via `capture="environment"` where supported.

## Deploy
- GitHub Pages / Netlify / Vercel: drag-drop or push this directory.
