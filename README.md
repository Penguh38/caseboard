# LSSD Case Board

A collaborative investigation board built for law enforcement roleplay communities. Pin suspects, victims, evidence and locations on a shared board — connect the dots and solve the case together.

![License](https://img.shields.io/badge/license-Proprietary-red.svg)
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

Copyright (c) 2025 Penguh38. All Rights Reserved.

This software and its source code are proprietary and confidential.
No part of this software may be reproduced, distributed, modified,
or used in any form without the prior written permission of the author.

Unauthorized use, copying, or distribution of this software,
via any medium, is strictly prohibited.
