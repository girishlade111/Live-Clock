# Live Clock

A minimal, real-time digital clock that runs entirely in your browser. No frameworks, no build step, no login — just open the page and it ticks.

## Features

- Live 24-hour digital clock (HH:MM:SS) updating every second
- Zero dependencies — plain HTML, CSS, and JavaScript
- Responsive centered layout that works on any screen size
- Runs fully client-side; no server, no tracking

## Tech stack

- HTML5
- CSS3
- Vanilla JavaScript (DOM + `setInterval`)

## Quick start

```bash
# clone and open
git clone https://github.com/girishlade111/Live-Clock.git
cd Live-Clock
# open index.html in any browser — no server needed
```

Or use a simple static server:

```bash
npx serve .
```

## Project structure

```
Live-Clock/
├── index.html    # page markup, loads styles and script
├── styles.css    # layout and clock styling
└── script.js     # clock update logic (updateClock every 1000ms)
```

## How it works

`script.js` reads the current time with `new Date()`, zero-pads hours/minutes/seconds, writes them into the `#clock` element, and refreshes every second via `setInterval`. An initial call renders the time immediately on page load.

## Deploy notes

Deployed as a static site on GitHub Pages: https://girishlade111.github.io/Live-Clock/

---

Built by Girish Lade — https://ladestack.in
