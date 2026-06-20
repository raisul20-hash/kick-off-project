# kick-off-project

Good Day Fellas,

This is my first portfolio repository. It documents how I set up this kick-off project using AI-assisted coding tools — what I installed, what I completed, and what problems came up along the way.

**Repository:** [github.com/raisul20-hash/kick-off-project](https://github.com/raisul20-hash/kick-off-project)

---

## Repository Structure

```
kick-off-project/
├── README.md
└── research/
    ├── sources.md                          # Curated expert list (10 practitioners)
    ├── youtube-transcripts/
    │   ├── julian-goldie.md
    │   ├── matt-diggity.md
    │   └── nathan-gotch.md
    └── linkedin-posts/
        ├── aleyda-solis/        (2 posts)
        ├── bernard-huang/       (2 posts)
        ├── brian-dean/          (2 posts)
        ├── gael-breton/         (2 posts)
        ├── julian-goldie/       (3 posts)
        ├── koray-tuğberk/       (3 posts)
        ├── mark-webster/        (2 posts)
        ├── matt-diggity/        (3 posts)
        ├── nathan-gotch/        (2 posts)
        └── ross-hudgens/        (2 posts)
```

Each LinkedIn post is stored as a dated markdown file (e.g. `2026-06-16_aeo-geo-vs-seo.md`) with the post text, source URL, and scrape metadata.

---

## Tools Installed

### Development environment

| Tool | Purpose | Status |
|------|---------|--------|
| **Cursor** | IDE for editing and running AI agents | Installed and in use |
| **Cursor Agent (Composer)** | AI pair-programming inside Cursor | Used to explore and write this repo |
| **Codex** | AI coding model in Cursor | Used for research docs and README updates |
| **Claude Code** | Terminal-based AI coding agent | Discussed as a next step for full repo scaffolding |
| **Git + GitHub** | Version control and remote hosting | Active — 32+ commits on `main` |

### Planned project stack (not installed yet)

These tools are defined in the project brief but **not yet set up** in this repo — there is no `package.json`, source code, or dependency install so far.

| Tool | Planned use |
|------|-------------|
| **Node.js** (≥ 20.x) | Runtime for frontend and backend |
| **npm** (workspaces) | Package manager and monorepo layout |
| **TypeScript** | Shared language across apps |
| **React 18 + Vite** | Frontend dev server and UI |
| **Express** | Backend API |
| **SQLite** (`better-sqlite3`) | Local database |
| **Vitest** | Unit and integration tests |
| **ESLint + Prettier** | Linting and formatting |
| **GitHub Actions** | CI on push/PR |

---

## Steps Completed

1. **Downloaded the repository** — Created local folder `kick-off-project-main` as a blank starter.
2. **Explored the project** — Confirmed the repo initially contained only a title and greeting; no app code or config files.
3. **Drafted a project brief** — Expanded the README with a full-stack plan: React + Vite frontend, Express API, SQLite, shared TypeScript types, tests, and CI.
4. **Defined project structure** — Documented intended layout (`apps/web`, `apps/api`, `packages/shared`, GitHub Actions workflow).
5. **Wrote setup and acceptance criteria** — Added install commands, dev workflow, API contract (`GET /api/health`), and a v1 checklist.
6. **Researched AI workflow** — Identified how to split work between Cursor/Codex (in-IDE edits) and Claude Code (terminal scaffolding from the README).
7. **Updated this README** — Refocused it as a portfolio log: tools used, progress, and issues encountered.
8. **Built SEO research corpus** — Added `research/` with a curated [sources.md](research/sources.md) covering 10 AI-SEO practitioners.
9. **Scraped YouTube transcripts** — Summarized key videos from Nathan Gotch, Matt Diggity, and Julian Goldie into markdown.
10. **Scraped LinkedIn posts** — Collected 23 posts across 10 experts, organized by author in `research/linkedin-posts/`.

---

## Research Highlights

| Category | Location | Content |
|----------|----------|---------|
| Expert index | [research/sources.md](research/sources.md) | 10 practitioners with annotated resource links |
| YouTube summaries | [research/youtube-transcripts/](research/youtube-transcripts/) | 3 video breakdowns (Gotch, Diggity, Goldie) |
| LinkedIn posts | [research/linkedin-posts/](research/linkedin-posts/) | 23 scraped posts from 10 SEO/AI experts |

---

## Issues Encountered and How They Were Solved

### 1. Empty repository with no direction

**Issue:** The repo started with almost no content — just a heading and "Good Day Fellas," — so there was no stack, structure, or setup to follow.

**Solution:** Used Cursor Agent to expand the README into a full project brief (stack, folder tree, setup steps, and acceptance criteria). That gave a clear target for the next implementation phase.

---

### 2. README did not match reality

**Issue:** The brief described files and commands (`npm install`, `npm run dev`, etc.) that do not exist yet. Anyone cloning the repo would hit errors immediately.

**Solution:** Split "planned stack" from "installed tools" in this README and marked scaffold items as **not yet installed**. Future step: implement the structure so the documented commands actually work.

---

### 3. Accidental placeholder text

**Issue:** A stray `testt` line appeared in an earlier README edit — likely a typo or test keystroke.

**Solution:** Removed the placeholder and replaced it with intentional, structured documentation.

---

### 4. Git not initialized locally

**Issue:** The local project folder was not a Git repository initially, so there was no commit history or remote tracking.

**Solution:** Repository is now live on GitHub with 32+ commits. Local clones should run `git clone https://github.com/raisul20-hash/kick-off-project.git` to sync.

---

### 5. Node.js / npm not verified for this project

**Issue:** Project dependencies were never installed because the codebase scaffold was not created. Node/npm may also need to be confirmed on the local machine before implementation.

**Solution:** Listed Node and npm under **planned** tools. Before scaffolding, verify with:

```bash
node -v   # expect ≥ 20.x
npm -v    # expect ≥ 10.x
```

Install from [nodejs.org](https://nodejs.org/) if either command is missing.

---

### 6. Choosing between Codex and Claude Code

**Issue:** Unclear which AI tool should do what — README edits vs full multi-file scaffolding.

**Solution:** Adopted a simple split:

- **Cursor / Codex** — Refine README, small edits, research docs, and in-IDE changes.
- **Claude Code** — One-shot scaffold from the README (`apps/`, `packages/`, configs, CI).

Prompt to use next: *"Implement everything described in README.md."*

---

### 7. Research files uploaded out of folder structure

**Issue:** Early YouTube transcript uploads landed at the repo root instead of under `research/youtube-transcripts/`.

**Solution:** Reorganized into the `research/` tree with separate folders for transcripts, LinkedIn posts, and the sources index.

---

## What's Next

- [x] Initialize Git and connect remote on GitHub
- [x] Build SEO research corpus (sources, YouTube transcripts, LinkedIn posts)
- [ ] Install Node.js and npm if not already available
- [ ] Scaffold the monorepo to match the planned structure
- [ ] Run `npm install`, `npm run dev`, `npm run test`, and `npm run lint`
- [ ] Update this README with **actual** installed versions and verified commands
- [ ] Continue scraping LinkedIn posts for remaining experts

---

## Planned v1 Goal (reference)

When implementation is done, v1 should be a **health-check dashboard**: the React frontend calls `GET /api/health`, the Express API responds with JSON, and tests + CI pass on a fresh clone.

---

*Last updated: June 21, 2026*
