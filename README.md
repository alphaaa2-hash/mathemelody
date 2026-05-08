# Mathemelody

A browser-based musical sequencer that transforms mathematical equations into melodies.
Each step in the sequence evaluates an equation using the step index as `x`, and maps
the result to a note on a C major scale.

## How it works

1. Set the number of steps and click **Update Grid**
2. Enter an equation in each cell using `x` as the step number
3. Select a wave type (sine, square, triangle, sawtooth)
4. Hit **Play** and listen

## Supported expressions

| Type | Examples |
|---|---|
| Basic arithmetic | `2*x + 1`, `x^2 - 3` |
| Trigonometric | `sin(x)`, `cos(x) * 4` |
| Logarithmic | `log(x)`, `ln(x)` |
| Constants | `pi`, `e` |
| Complex numbers | `i^x`, `re(i^x)` |

> For complex results, the **magnitude** is used to determine the note played.

## Controls

- **Tempo** — adjust BPM with the slider
- **Wave type** — changes the timbre of each note
- **Dark mode** — toggle in the top controls

## Built with

- [Web Audio API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)
- [mathjs](https://mathjs.org)
- [Chart.js](https://www.chartjs.org)

## Try it

Open `index.html` in any modern browser — no install needed.
