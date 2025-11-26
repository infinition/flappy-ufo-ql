# FLAPPY UFO: Deep-Dive Q-Learning Trainer

![Version](https://img.shields.io/badge/Status-RL_Trainer-00f3ff?style=for-the-badge)
![Tech](https://img.shields.io/badge/Tech-Canvas%20%7C%20Vanilla_JS-2ecc71?style=for-the-badge)


**A high-performance, zero-dependency visualization of Reinforcement Learning running entirely in your browser.**

Watch the  **AI agent** learn to navigate the environments using the Q-Learning algorithm. customize the world, tweak the hyperparameters on the fly, and hit **Turbo Mode** to train thousands of episodes in seconds.

-----

### 🌐 Live Demo
Experience the trainer instantly: https://infinition.github.io/flappy-ufo-ql/

-----
<img width="1158" height="1279" alt="image" src="https://github.com/user-attachments/assets/1af40a42-0cbd-4c58-a49c-7a5cfb3b048c" />

## 🚀 Key Features & Performance

  * **High-Speed Training:** The **Speed Multiplier** lets you run the simulation up to **x1000** by decoupling the logic loop from rendering, ensuring maximum simulation speed for rapid iteration.
  * **Real-time Tuning:** Adjust the core Q-Learning parameters ($\epsilon, \alpha, \gamma$) instantly.
  * **Physics Modulator:** Change **Gravity**, **Jump Force**, and pipe parameters on the fly to challenge the agent with new environmental rules.
  * **Robust Mode:** Toggle randomized physics settings upon each reset to force the AI to learn a generalized, robust policy.
  * **Persistent Learning:** **Export/Import** the entire Q-Table (`flappy_brain.json`) to save and share trained models.

-----

## 🧠 Q-Learning Parameters & Feedback

The simulator uses a discretized state representation for Q-Learning, where the state is based on: **Horizontal distance to the next pipe**, **Vertical distance to the gap center**, and **UFO's current velocity**.

  * **Live Neural Feedback:** A visible **NEURAL OUTPUT LED** confirms the AI's "JUMP" action in real-time.
  * **Visual Debugging:** Toggle lines to show the agent's current target calculation (distance to the pipe center).
  * **Generational Charting:** Track the learning curve (Score per Generation) with controls for **Zoom** and **Smoothing** via the Chart.js graph.

-----

## 💻 Quick Start

**This project is a single-file application.**

1.  Download the `index.html` file.
2.  Open it directly in any modern web browser.
3.  Click the screen or press **Space** to start the simulation.

### Game Modes

| Mode | Control | Description |
| :--- | :--- | :--- |
| **AI Auto** | Set Speed \> x1 | The Q-Learning algorithm controls the UFO, updates its Q-Table, and trains itself. |
| **Human Player** | Toggle Player Mode | You control the UFO (click/spacebar). AI training and learning stop while in this mode. |

-----

## 🛠️ Tech Stack

  * **Single-File Architecture:** Everything (HTML/CSS/JS) is contained in one portable file.
  * **HTML5 Canvas:** Used for efficient game rendering.
  * **Vanilla JavaScript:** Core physics and Q-Learning logic is implemented without external libraries.
  * **Chart.js:** Used for live analytic plotting.

**License:** MIT. Free to use and modify.
