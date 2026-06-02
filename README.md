# Flappy UFO: Q-Learning Trainer

[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black) [![Release](https://img.shields.io/github/v/release/infinition/flappy-ufo-ql?style=flat)](https://github.com/infinition/flappy-ufo-ql/releases) [![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-ffdd00?style=flat&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/infinition)

A browser-based Q-Learning visualizer built around a Flappy Bird variant. Watch an agent learn to fly through pipes, tune hyperparameters live, and run thousands of episodes in seconds with the speed multiplier.

Live: https://infinition.github.io/flappy-ufo-ql/

![Flappy UFO](https://github.com/user-attachments/assets/307b72e2-e8af-4e86-b618-25c633ffb514)

<img width="1158" height="1279" alt="Flappy UFO trainer" src="https://github.com/user-attachments/assets/1af40a42-0cbd-4c58-a49c-7a5cfb3b048c" />

---

## How it works

The agent receives a discretized state: horizontal distance to the next pipe, vertical distance to the gap center, and current velocity. It picks actions from a Q-table updated via the standard Q-Learning rule with configurable epsilon, alpha, and gamma.

The speed multiplier decouples the logic loop from rendering, allowing up to x1000 speed for fast policy convergence without freezing the UI.

---

## Features

- Speed multiplier up to x1000 for rapid training.
- Live tuning of epsilon, alpha, and gamma without restarting.
- Physics modulator: adjust gravity, jump force, and pipe parameters mid-run.
- Robust Mode: randomizes physics on each reset to force a more generalized policy.
- Export and import the full Q-table as `flappy_brain.json`.
- Generation chart with zoom and smoothing controls (Chart.js).
- Human player mode (click or Space to control the UFO manually).
- Neural output LED showing the agent's jump decision in real time.

---

## Running

Single-file application. Download `index.html` and open it in any modern browser.

---

## Stack

- Vanilla JavaScript, HTML5 Canvas
- Chart.js for live analytics
- No dependencies, no build step

---

## Star History

<a href="https://www.star-history.com/?repos=infinition%2Fflappy-ufo-ql&type=date&legend=top-left">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chart?repos=infinition/flappy-ufo-ql&type=date&theme=dark&legend=top-left" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chart?repos=infinition/flappy-ufo-ql&type=date&legend=top-left" />
   <img alt="Star History Chart" src="https://api.star-history.com/chart?repos=infinition/flappy-ufo-ql&type=date&legend=top-left" />
 </picture>
</a>

---

## License

MIT.
