# Umang 2025 Website

![Project](https://img.shields.io/badge/Project-Umang%202025-0077b6)
![Site Type](https://img.shields.io/badge/Site-Static%20HTML%2FCSS%2FJS-0a9396)
![Build](https://img.shields.io/badge/Build-Manual-lightgrey)
![Version](https://img.shields.io/badge/Version-2025-blue)
![License](https://img.shields.io/badge/License-Not%20Specified-lightgrey)

Official website codebase for **Umang '25**, IIIT Bangalore's flagship inter-college sports fest.

This repository contains a static, multi-page event website with dedicated sport pages, event information, registration links, team details, and contact information.

## Table of Contents

- [What This Project Does](#what-this-project-does)
- [Why This Project Is Useful](#why-this-project-is-useful)
- [Project Structure](#project-structure)
- [How to Get Started](#how-to-get-started)
- [Usage Examples](#usage-examples)
- [Where to Get Help](#where-to-get-help)
- [Who Maintains and Contributes](#who-maintains-and-contributes)
- [Contributing](#contributing)
- [Notes](#notes)

## What This Project Does

The project powers the Umang 2025 sports fest website, including:

- Landing page with event branding and hero section (`index.html`)
- Events listing page (`events.html`)
- Individual sport pages (for example `football.html`, `basketball.html`, `badminton.html`)
- Team and organizer pages (`team.html`, `contact.html`)
- Shared frontend assets under `assets/` (CSS, JS, images, fonts)
- Maintenance scripts for updating and validating sport pages

## Why This Project Is Useful

- Fast to deploy: no build step is required for core website pages.
- Easy to maintain: each sport has its own page and can be edited independently.
- Consistent design workflow: helper scripts support batch updates and verification.
- Contributor-friendly structure: clear top-level HTML pages and centralized assets.
- Event-ready content model: sport rules, registration links, contacts, and visuals are already integrated.

## Project Structure

```text
.
|-- index.html
|-- events.html
|-- team.html
|-- contact.html
|-- football.html
|-- basketball.html
|-- badminton.html
|-- chess.html
|-- kabaddi.html
|-- tabletennis.html
|-- tennis.html
|-- throwball.html
|-- volleyball.html
|-- assets/
|   |-- css/
|   |-- js/
|   |-- img/
|   |-- fonts/
|   `-- scss/
|-- update_sports_pages.py
|-- update_sports_theme.py
|-- verify_sports_pages.py
|-- update_all_sports.js
`-- update_all_sports.ps1
```

## How to Get Started

### Prerequisites

- A modern browser (Chrome, Edge, Firefox, Safari)
- Python 3.8+ (optional, for Python maintenance scripts)
- Node.js 16+ (optional, for Node scripts)
- PowerShell 5.1+ on Windows (optional, for `.ps1` script)

### 1. Clone the repository

```bash
git clone <your-repo-url>
cd Umang2025
```

### 2. Run locally

Option A: Open `index.html` directly in your browser.

Option B (recommended): Serve via a local HTTP server.

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

### 3. Edit pages

- Update top-level page content directly in the corresponding `.html` files.
- Add or replace images in `assets/img/`.
- Update shared styles in `assets/css/`.

## Usage Examples

### Validate sports pages after edits

```bash
python verify_sports_pages.py
```

### Batch update sports pages from template logic

```bash
python update_sports_pages.py
```

### Run JavaScript helper script

```bash
node update_all_sports.js
```

### Run PowerShell helper script (Windows)

```powershell
.\update_all_sports.ps1
```

## Where to Get Help

- Organizer contact page: `contact.html`
- Team and owners context: `team.html`
- Primary support email used across pages: `sportscomm@iiitb.ac.in`
- Event and registration navigation: `events.html`

If you are contributing and unsure where to make a change, start from `events.html` and the related sport page, then verify with `verify_sports_pages.py`.

## Who Maintains and Contributes

Maintained by the **Umang / Sports Committee, IIIT Bangalore**.

Current organizer and contributor details are published on:

- `team.html`
- `contact.html`

## Contributing

Contributions are welcome for content updates, design improvements, accessibility fixes, and page consistency.

Suggested workflow:

1. Create a feature branch.
2. Make focused edits in related page(s) and assets.
3. Run `python verify_sports_pages.py` for sports-page checks.
4. Open a pull request with a summary of changes, screenshots for UI changes, and manual validation notes.

For larger collaboration, add a dedicated contribution guide at `CONTRIBUTING.md` and link it here.

## Notes

- This repository currently does not include a `LICENSE` file.
- No CI pipeline is configured in the current workspace, so the build badge reflects manual checks.
