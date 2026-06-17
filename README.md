# kick-off-project

Good Day Fellas,

This is my first portfolio repository. It documents how I set up this kick-off project using AI-assisted coding tools — what I installed, what I completed, and what problems came up along the way.

---

## Tools Installed

### Development environment

| Tool | Purpose | Status |
|------|---------|--------|
| **Cursor** | IDE for editing and running AI agents | Installed and in use |
| **Cursor Agent (Composer)** | AI pair-programming inside Cursor | Used to explore and write this repo |
| **Codex** | AI coding model in Cursor | Discussed and planned with; not yet used to scaffold code |
| **Claude Code** | Terminal-based AI coding agent | Discussed as a next step for full repo scaffolding |

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
| **Git** | Version control |

---

## Steps Completed

1. **Downloaded the repository** — Created local folder `kick-off-project-main` as a blank starter.
2. **Explored the project** — Confirmed the repo initially contained only a title and greeting; no app code or config files.
3. **Drafted a project brief** — Expanded the README with a full-stack plan: React + Vite frontend, Express API, SQLite, shared TypeScript types, tests, and CI.
4. **Defined project structure** — Documented intended layout (`apps/web`, `apps/api`, `packages/shared`, GitHub Actions workflow).
5. **Wrote setup and acceptance criteria** — Added install commands, dev workflow, API contract (`GET /api/health`), and a v1 checklist.
6. **Researched AI workflow** — Identified how to split work between Cursor/Codex (in-IDE edits) and Claude Code (terminal scaffolding from the README).
7. **Updated this README** — Refocused it as a portfolio log: tools used, progress, and issues encountered.

---

## Issues Encountered and How They Were Solved

### 1. Empty repository with no direction

**Issue:** The repo started with almost no content — just a heading and “Good Day Fellas,” — so there was no stack, structure, or setup to follow.

**Solution:** Used Cursor Agent to expand the README into a full project brief (stack, folder tree, setup steps, and acceptance criteria). That gave a clear target for the next implementation phase.

---

### 2. README did not match reality

**Issue:** The brief described files and commands (`npm install`, `npm run dev`, etc.) that do not exist yet. Anyone cloning the repo would hit errors immediately.

**Solution:** Split “planned stack” from “installed tools” in this README and marked scaffold items as **not yet installed**. Future step: implement the structure so the documented commands actually work.

---

### 3. Accidental placeholder text

**Issue:** A stray `testt` line appeared in an earlier README edit — likely a typo or test keystroke.

**Solution:** Removed the placeholder and replaced it with intentional, structured documentation.

---

### 4. Git not initialized

**Issue:** The project folder is not a Git repository (no `.git` directory), so there is no commit history or remote tracking yet.

**Solution:** Documented as an open item. Next step: run `git init`, add a `.gitignore`, make an initial commit, and connect a remote when ready.

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

- **Cursor / Codex** — Refine README, small edits, and in-IDE changes.
- **Claude Code** — One-shot scaffold from the README (`apps/`, `packages/`, configs, CI).

Prompt to use next: *“Implement everything described in README.md.”*

---

## What’s Next

- [ ] Install Node.js and npm if not already available
- [ ] Initialize Git and add `.gitignore`
- [ ] Scaffold the monorepo to match the planned structure
- [ ] Run `npm install`, `npm run dev`, `npm run test`, and `npm run lint`
- [ ] Update this README with **actual** installed versions and verified commands

---

## Planned v1 Goal (reference)

When implementation is done, v1 should be a **health-check dashboard**: the React frontend calls `GET /api/health`, the Express API responds with JSON, and tests + CI pass on a fresh clone.

---

*Last updated: June 17, 2026*
