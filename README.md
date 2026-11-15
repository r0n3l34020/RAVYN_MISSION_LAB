# 🚀 RAVYN MISSION LAB
### NASA Space Apps Challenge | Space Mission Design Game

**RAVYN MISSION LAB** is an award-contending 2.5D retro systems-engineering RPG inspired by the visual aesthetic of *Pokémon White 2*. Players step into the shoes of a Rookie Systems Engineer at a NASA-inspired facility, guiding a spacecraft across an immersive **4-Act Campaign** that covers all four official NASA mission segments and transitions through JPL Concept Maturity Levels (CML 1–4).

The game combines vibrant pixel-art top-down exploration with high-stakes, physics-driven mini-games, replacing dry text dialogues with tactile engineering challenges.

---

## 🎮 Gameplay Structure: The 4-Act Campaign
The game is divided into four distinct acts, mapping directly to NASA's mission segments and JPL CML frameworks:

### **Act 1: Launch Segment (The Launch Complex) — CML 1**
* **Top-Down Map:** A fenced launch pad compound featuring a cryogenic fueling depot, umbilical tower, and concrete blockhouse bunker.
* **Task 1 (Cryogenic Fueling & Boil-Off):** Liquid oxygen (LOX) boils off as it warms up, building dangerous tank pressure. Players manage pad valves to top off the fuel gauge while hitting a "Vent" valve whenever pressure hits the red zone in a frantic countdown race.
* **Task 2 (Max-Q Throttle Management):** Inside the bunker console, a live side-profile rocket meter displays structural vibrations building during Maximum Aerodynamic Pressure. Players pull the throttle lever into a green "safe zone" through the cloud layer, then slam it back to 100% once clear.

### **Act 2: Space Segment (Orbital Deployment) — CML 2**
* **Top-Down Map / Orbital View:** Zero-G orbital space around the newly deployed satellite chassis (complete with blue solar panels, red radiator fins, and visible thruster nodes).
* **Task 1 (Detumbling Physics Puzzle):** The satellite spins freely in 2D space. Players tap directional thrusters opposite the spin vectors until rotation hits 0.0°/s using conservation of angular momentum.
* **Task 2 (Solar Array & Thermal Orientation):** Sunlight streams from one side of the screen. Players rotate the satellite so blue solar panels catch the light beams (charging the battery) while keeping sensitive red radiator fins turned away toward deep space shadow.

### **Act 3: Ground Segment (Mission Control & DSN Array) — CML 3**
* **Top-Down Map:** Mission Control floor with glowing console desks and an outdoor satellite dish field visible through reinforced glass windows.
* **Task 1 (Line-of-Sight Pass & Signal Lock):** Incorporates GMAT two-body orbital mechanics ($v = \sqrt{\mu/r}$, $T = 2\pi\sqrt{r^3/\mu}$). A radar map displays a shrinking pass window; players align an antenna dish toward the moving blip and tune a frequency slider until two Doppler waveforms overlap into a clean sine wave.
* **Task 2 (Uplink Packet Prioritization):** A 30-second signal timer counts down while players drag high-priority command blocks into a limited upload queue before the satellite drops below the horizon.

### **Act 4: User Segment (The Science Lab) — CML 4**
* **Top-Down Map:** Research laboratory featuring server racks, spectrometer desks, and a holographic planet table.
* **Task 1 (Spectral Filtering & Noise Removal):** Raw space data is obscured by cosmic-ray static. Players toggle three scientific filters (Infrared, Noise Reduction, Contrast Calibration) to reveal hidden features like an exoplanet dip.
* **Task 2 (Discovery Classification & Re-Tasking):** Players match cleaned wavelength spikes against a field guide poster (matching lines to $H_2O$ or Methane), stamp the official discovery report, and select target coordinates.
* **Mission Debrief Card:** Grades overall performance across all four acts, showing how earlier decisions (like Act 1 fuel efficiency or Act 3 signal lock) directly impact final telemetry and data clarity.

---

## 🧪 NASA Data & Framework Alignment
* **Concept Maturity Levels (CML 1–4):** Tracks progressive mission milestones from initial concept (CML 1) through trade studies (CML 2), point design (CML 3), and operational demonstration (CML 4).
* **Astrodynamics Kernels:** Utilizes real GMAT two-body equations, LOX boil-off thermodynamics, and Doppler shift calculations.
* **Modular Asset Architecture:** Configured with centralized stubs for 4-directional character sprites (`sprites: { down, up, left, right }`) and interchangeable rocket/instrument parts.

---

## 🛠️ Technology & Architecture
* **Single-File Architecture:** 100% self-contained in a single `index.html` file with zero external dependencies (HTML5 Canvas, CSS3, ES6+ JavaScript).
* **Procedural Audio:** Custom WebAudio synthesizer generating real-time 8-bit sound effects, rocket rumbles, and 4 dynamic background music loops.
* **Visuals:** 2.5D retro pixel-art aesthetic with Y-sorted sprite rendering.

---

## ▶️ How to Run
### **Live Play — GitHub Pages**
Open the hosted repository URL in any modern desktop browser:
[https://<github-username>.github.io/<repository-name>/](https://<github-username>.github.io/<repository-name>/)
*(No installation, build step, or server required).*

### **Local Execution — Offline**
1. Clone the repository:
   ```bash
   git clone [https://github.com/](https://github.com/)<github-username>/<repository-name>.git
   ```
2. Open the folder and double-click index.html to launch locally in your browser.

### Controls

| Action              | Control               |
|---------------------|-----------------------|
| Walk / Navigate     | W A S D or Arrow Keys |
| Interact / Select   | E, Spacebar, or Enter |
| Close Modals / Exit | Esc                   |
| Open NASA Codex     | C                     |
| Audio / Mute        | Top HUD buttons       |

## 👥 Team RAVYN & Credits
- **Ronel Jonathan** - Systems Architect & Core Gameplay Coder
- **Yaron Emmanuel Sebastian** — Visual Director & Slide Deck Design
- **Shri Arjun Karthik** — Technical Documentation Specialist & Research
- **Vedanth Achanta** — Character & Asset Art Design

## 🤖 Note on AI Collaboration & Development
Building an ambitious, 100-percent self-contained retro RPG simulation within a tight hackathon timeframe required a robust human-AI collaboration workflow across the entire team.

_Core Systems Architecture & Code_: Developed primarily using Google AI Studio (Gemini 4 Hydrogen model) running on high-thinking capacity, leveraging its advanced logic and problem-solving capabilities to architect the single-file HTML5 canvas engine, procedural WebAudio synth, and interactive mini-games. ChatGPT was occasionally used for rapid code touch-ups and syntax polishing, while Gemini (Auto mode at Medium/High thinking) served as an interactive coding partner for brainstorming and live debugging.

_Visual Direction & Asset Design_: AI tools like Gemini were used to generate character concept blueprints and mood boards, but the team's asset designer hand-crafted every final pixel-art character and interface element. Gemini also provided layout and structural inspiration for the presentation slide deck.

_Research & Documentation_: Team members utilized ChatGPT and Gemini to cross-reference aerospace engineering concepts, refine GitHub documentation, and organize project specifications.

Ultimately, while AI accelerated the engineering and prototyping pipeline, the architectural design, gameplay mechanics, integration, and final polishing were driven entirely by human direction and teamwork.

### 📄 Attribution & Disclaimer
Developed for the NASA Space Apps Challenge. References to NASA, JPL, GMAT, and DSN are used for educational context. The project is not affiliated with or endorsed by NASA or JPL. Visual direction draws inspiration from retro handheld RPGs. Uses MIT License. 
