# Zenthi

**Rare parts. Real fixes. Built from scratch.**

Zenthi is a free, community-run archive of car-part files — retrofits, fixes, and hard-to-find parts for any vehicle.

The hardest, most inventive fixes tend to come from high-performance and exotic builds pushing into territory nobody else supports, but the same spirit applies to any car with a rare problem to solve. A discontinued clip for a daily driver is just as welcome as a one-off fix for an exotic.

Completely free. No paywall. If you've ever solved an obscure fitment problem yourself, this is a place to put it where the next person doesn't have to start from zero.

---

## Features

### Library
Browse and download community-submitted files, filterable by make, model, year, engine, drivetrain, and category.

### Upload
Submit a file — STEP, STL, OBJ, PLY, DXF, SVG, PDF, native CAD, and more. Tag vehicle fitment, note material and thickness, and credit the original source if you're reuploading or modifying someone else's work.

### Requests board
Post a part you need scanned or modeled; others can fulfill it publicly, under review, or privately to you.

> No payment processing. Any financial agreement between users happens off-platform.

### Web search
Structured fitment search across external sources via the Brave Search API. Returns titles, snippets, and links only — Zenthi never downloads, stores, or rehosts files it doesn't have direct permission for.

---

## Licensing & attribution

Every upload requires an explicit license choice and honest sourcing.

**Available licenses:** CC0, CC BY, CC BY-SA, CC BY-NC, CC BY-ND, CC BY-NC-ND

| Submission type | What's required |
| --- | --- |
| Original work | Licensed CC BY by default |
| Reuploaded from elsewhere | Source link, original license, creator credit |
| Modified from someone else's file | All of the above, plus a description of what changed |

Two rules are enforced automatically:

- Submissions are **blocked** if the original license doesn't permit derivatives (ND variants).
- **ShareAlike (SA)** licenses propagate to the new upload.

See [`/copyright-policy`](/copyright-policy) for the full takedown process.

---

## Scope & safety

Nothing is restricted by vehicle type or part category.

> ⚠️ **Safety-critical parts** — brakes, suspension, structural, fuel system — are **fitment reference only**, not verified functional replacements. See the homepage and footer disclaimer for the full framing.

---

## Community governance

Zenthi is moving toward being community-run.

Anyone can create an account (email/password, GitHub, or Google) to upload, post requests, or fulfill them.

Admin access is granted by request — existing admins review and approve new admin requests. Nobody can self-promote.

See [`/community-guidelines`](/community-guidelines) for what's expected of contributors and admins.

---

## Tech stack

| Layer | Stack |
| --- | --- |
| Frontend | React, TanStack Router / Start |
| Backend | Supabase — Postgres, Auth, Storage, Row-Level Security |
| Search | Brave Search API |
| Hosting / build | Lovable |

---

## Contributing

Upload a file, post a request, or just browse. If you find a bug or have a suggestion, open an issue.

This project was shaped almost entirely by real user feedback — keep it coming.
