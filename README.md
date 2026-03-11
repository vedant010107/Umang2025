# Umang 2025 Website

Official website for **Umang '25**, IIIT Bangalore's inter-college sports fest.

This is a static website with pages for events, individual sports, team details, and contact information.

## What This Project Does

- Showcases Umang 2025 event information and highlights.
- Lists all sports and competition categories.
- Provides separate pages for each sport with rules and registration links.
- Displays organizing team details and contact information.

## Why This Project Is Useful

- Simple and fast static website setup.
- Easy to update page-wise content for each sport.
- Organized structure with reusable assets in `assets/`.
- Suitable for fest publicity, participant info, and registrations.

## Main Pages

- `index.html` - Home page
- `events.html` - Sports/events list
- `football.html`, `basketball.html`, `badminton.html`, `chess.html`, `kabaddi.html`, `tabletennis.html`, `tennis.html`, `throwball.html`, `volleyball.html` - Sport-specific pages
- `team.html` - Organizing team
- `contact.html` - Contact details

## Project Structure

```text
.
|-- index.html
|-- events.html
|-- team.html
|-- contact.html
|-- <sport>.html pages
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

## Contributing

Contributions are welcome for:

- Content updates
- UI improvements
- Responsiveness and accessibility fixes
- Sports page consistency updates
