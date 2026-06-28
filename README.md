# Roster — employer-side prototype (v1)

Clickable static prototype for an AI hiring-agent product. The agent unit is a **Recruiter**: one Recruiter runs one role end to end — sources candidates, books interviews, conducts them on-platform, takes notes. (Names are working names.)

## Pages
- `index.html` — dashboard: Recruiter cards (interviews / scheduled / hires), free-trial strip, New Recruiter.
- `create.html` — 3-step create flow: role + AI-drafted JD + must-haves → availability → review → launch.
- `recruiter.html` — one role's matched candidates with match-score bars + role/sourcing side panel.
- `candidate.html` — resume, accept/decline (decline confirm), messaging, Accept & schedule.
- `interview.html` — on-platform interview room: video tiles, controls, timer, notes, End & rate.

## Stack
Static HTML/CSS/JS, mock data only, no backend. State persists in `sessionStorage`.
Shared `assets/app.css` + `assets/app.js`. `.nojekyll` included for GitHub Pages.

## Scope (v1, employer side)
No real matching engine, no auth/resume upload, no rescheduling (v2), no agent-learning-from-ratings (v2/v3 — ratings are captured but don't drive matching). Candidate-side screens come next.

## Run locally
Open `index.html` in a browser, or: `python3 -m http.server` then visit the printed URL.
