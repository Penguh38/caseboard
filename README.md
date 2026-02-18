#Case Board

A collaborative investigation board built for law enforcement roleplay communities. Pin suspects, victims, evidence and locations on a shared board — connect the dots and solve the case together.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Node](https://img.shields.io/badge/node-%3E%3D18-green.svg)

---

## Features

- **14 pin types** — Suspect, Victim, Witness, Evidence, Vehicle, Weapon, Officer, and more
- **Connection strings** — link pins with labeled lines in solid, dashed, or dotted styles
- **Interactive map board** — place markers, draw territory zones, and connect locations
- **Real-time collaboration** — changes sync automatically across all connected users
- **Share links** — share cases with view-only or edit permissions via a single link
- **Sticky notes** with checkboxes for tracking leads and tasks
- **User profiles** — set your name, rank, and badge number per session
- **Agency themes** — switch between LSPD, LSSD, LSFD, SADOC, and SANFIRE branding
- **Zoom controls**, collapsible sidebar, and keyboard shortcuts
- **No account required** — just open and start working

---

## Tech Stack

- **Backend** — Node.js, Express
- **Frontend** — Vanilla JavaScript, no frameworks, no build step
- **Storage** — Vercel KV (Redis) in production / JSON file locally

---

## Getting Started

### Requirements

- Node.js v18+

### Run locally

```bash
git clone https://github.com/Penguh38/caseboard.git
cd caseboard
npm install
npm start
```

Open **http://localhost:3000** — data saves to `data.json` automatically, no database needed.

---

## Configuration

All config is done via environment variables. Copy `.env.example` to `.env` to get started.

| Variable | Default | Description |
|---|---|---|
| `PORT` | `3000` | Port the server runs on |
| `KV_REST_API_URL` | — | Vercel KV endpoint (production only) |
| `KV_REST_API_TOKEN` | — | Vercel KV auth token (production only) |

---

## Project Structure

```
caseboard/
├── server.js        # Express backend
├── vercel.json      # Deployment config
├── package.json
├── .env.example
└── public/
    ├── index.html   # Full frontend — single file
    └── logos/       # Agency logos
```

---

## License

MIT License

Copyright (c) 2025 Penguh38

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
