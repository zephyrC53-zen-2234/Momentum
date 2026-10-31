# Momentum

Momentum is a responsive calisthenics training app for learning bodyweight skills, following structured workouts, and tracking progress over time.

**Live app:** [zephyrc53-zen-2234.github.io/Momentum](https://zephyrc53-zen-2234.github.io/Momentum/)

## Features

- Skill progression paths from bodyweight foundations to muscle-ups
- Clear technique cues, prerequisites, targets, and common mistakes
- Progress tracking saved in the browser
- Beginner, skill, push/pull, and core workout routines
- Set-by-set workout tracking and a training journal
- Skill stopwatch with lap tracking
- Configurable rest timer
- Responsive layout for desktop and mobile

## Run locally

Clone the repository and start a local static server:

```bash
git clone https://github.com/zephyrC53-zen-2234/Momentum.git
cd Momentum
python3 -m http.server 4173 --directory dist
```

Open [http://localhost:4173](http://localhost:4173) in your browser.

No package installation or build step is required.

## Project structure

```text
Momentum/
├── dist/
│   ├── index.html       # App structure and training content
│   ├── momentum.css     # Responsive visual design
│   └── momentum.js      # Tracking, timers, and interactions
└── .github/workflows/
    └── pages.yml        # GitHub Pages deployment
```

## Progress storage

Momentum stores completed skill steps, workout sets, and session history in the browser using `localStorage`. Progress stays on the current device and browser. Clearing browser storage resets it.

## Deployment

Pushes to the `main` branch automatically publish the contents of `dist` through GitHub Actions and GitHub Pages.

```bash
git add .
git commit -m "Update Momentum"
git push
```

## Built with

- HTML
- CSS
- Vanilla JavaScript
- GitHub Actions and GitHub Pages

## License

No license has been added yet. All rights are reserved by default.
