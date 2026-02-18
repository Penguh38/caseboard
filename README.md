#Case Board

A collaborative investigation board built for law enforcement roleplay communities. Create case boards with pins, evidence threads, and an interactive map — all saved locally in your browser.

**[Live Demo →](https://your-deployment.vercel.app)**

---

## Features

- **14 pin types** — Suspect, Victim, Witness, Evidence, Vehicle, Weapon, and more
- **Connection strings** — link pins with labeled connections in solid, dashed, or dotted styles
- **Interactive map board** — drop markers, draw zones, and connect locations on a custom map
- **Multiple cases** — create and switch between separate investigation boards
- **Sticky notes** with checkboxes for tracking tasks
- **User profiles** — name, rank, and badge number per session
- **Agency branding** — switch between LSPD, LSSD, LSFD, SADOC, and SANFIRE themes
- **Keyboard shortcuts**, zoom controls, and a collapsible sidebar
- **Persistent storage** — all data saved in your browser, nothing sent to a server

---

## Tech Stack

- **Frontend** — Vanilla JavaScript, no frameworks, no build step
- **Storage** — Browser localStorage
- **Deployment** — Vercel (static)

---

## Deploy to Vercel

### Option 1 — Vercel CLI (fastest)

```bash
npm install -g vercel
vercel
```

Done. Vercel detects it as a static site automatically.

### Option 2 — GitHub + Vercel Dashboard

1. Push to GitHub:

```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/YOUR_USERNAME/caseboard.git
git push -u origin main
```

2. Go to [vercel.com](https://vercel.com) → **New Project** → import your repo → **Deploy**

No environment variables, no database, no configuration needed.

---

## Local Development

```bash
# Option 1 — any static server
npx serve .

# Option 2 — Python
python3 -m http.server 3000
```

Open **http://localhost:3000**

---

## Project Structure

```
caseboard/
├── public/
│   ├── index.html     # Full application — single file, no build step
│   └── logos/         # Agency logos
└── README.md
```

---

## Data & Privacy

All case data is stored in your browser's localStorage. Nothing is sent to any server. Clearing browser data will erase your cases.

---

## License

MIT
