# Rubik's Cube Lab

An interactive 3D Rubik's cube that runs in the browser. Scramble it, get a step-by-step CFOP solution right away, and race it with your real cube.

**Try it: https://michitruste.github.io/rubik/**

![Rubik's Cube Lab](og-image.png)

## Features

- **3D cube**: drag to orbit, scroll or pinch to zoom. It is only turned by scrambles and the solution, never by hand.
- **Random scrambles** (22 moves, Singmaster notation), always from a solved cube, that you can copy and go back to.
- **Race the CFOP solution**: solve your real cube while the solution plays on screen, and keep your times (best, ao5, ao12, wins).
- **CFOP solver** that runs as soon as a scramble finishes and shows the cross, the four F2L pairs, OLL and PLL. Play it all at once or step by step, with a diagram for each step.
  - *Human-style* or *fewest moves* solutions, with any cross color.
  - Choose which OLL and PLL cases and algorithms it may use: the full 1-look set, the 2-look beginner set, or your own. Export your choices to a file and import them again.
- **Flat net** of all six faces, a move history and a timer.
- Light and dark themes, and it works on phones.

## Keyboard

| Keys | Action |
| --- | --- |
| `S` | Scramble (resets the cube first) |
| Hold and release `Space` | Race the CFOP solution; any key stops your time |
| `←` `→` | Step one solution move |
| `Backspace` | Undo |

## Running locally

Everything is in one file, `index.html`, and the only dependency is [three.js](https://threejs.org/), loaded from a CDN. Serve the folder with any static server:

```bash
python -m http.server 8765
```

Then open http://localhost:8765/.
