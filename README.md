# Blush — Social App (React + Vite)

A responsive, pink-and-white social UI inspired by the supplied multi-screen design. Functional frontend demo runs independently of a backend; local state persists using browser `localStorage`.

## Quick start (Windows/macOS/Linux)

Install Node.js 20+ and run:

```bash
npm install
npm run dev
```

Open the localhost URL shown by Vite (usually http://localhost:5173).

## Production build

```bash
npm run build
npm run preview
```

## Deploy to Vercel

1. Upload this repository to GitHub, or import the folder using Vercel CLI.
2. In Vercel, choose **New Project**, import the GitHub repo.
3. Framework preset: **Vite**. Build command: `npm run build`. Output: `dist`.
4. Deploy. `vercel.json` already handles client-side route rewrites.
5. **No backend or environment variables are required** for the demo.

## Working frontend demo

- Home feed, stories strip, following-only filter
- Like/unlike, save/unsave, comment, and share link
- Search users, demo sound catalog and posts
- Follow/unfollow creators; individual profile pages
- Edit profile (name and bio)
- Chat conversations and send messages locally
- Notifications; discover images and hashtags
- Reels-like visual feed with prev/next, likes and saves
- Create a new post with a caption and optional image; preview videos
- Reset local demo data via profile settings
- Responsive desktop, tablet, and mobile layouts

## Important demo limitations

- This is a **frontend demo**, not a deployed social network with accounts, shared database, live chat or an API.
- Changes live in **this browser's localStorage**, not across devices/users. Clearing browser storage resets the demo.
- Uploaded images and short videos up to 900 KB are stored as data URLs in this browser, subject to browser storage quotas. Full video hosting/streaming requires backend or media service integration.
- People, counts, posts, music titles and notifications are fictional seeded demo records. No licensed music audio is streamed.
- Sample photos load from Unsplash and the typeface loads from Google Fonts, so images/fonts require an internet connection.
- For a full production version add auth, database, object storage, access rules, video processing, real-time chat and upload moderation. Integrate by replacing local state (`src/main.jsx`) with API calls.

## Architecture

- `src/main.jsx` — responsive pages, UI components and interactive demo state
- `src/data.js` — curated seed records
- `src/style.css` — all responsive design
- `vercel.json` — Vercel SPA rewrites

Made for demo and design reference purposes.
