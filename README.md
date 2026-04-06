# randomHTMLapps

A compendium of standalone browser apps built as single-file HTML experiences (HTML + CSS + JavaScript, no build step). Most are retro-inspired games, but there are also interactive simulations, audio tools, and creative utilities.

## Quick start

- Clone/download this repo.
- Open any `*.html` file directly in a modern browser, **or** serve the folder with a simple static server.
- If an app asks for microphone access, approve the browser permission prompt.

Example static server options:

```bash
python3 -m http.server 8080
# then open http://localhost:8080
```

```bash
npx serve .
```

## Application index

### Arcade & game experiences

- **`breakout.html` — Neon Breakout**  
  Brick-breaker with level progression, power-ups, and arcade-style glow visuals. Keyboard and touch controls are supported.

- **`galaxians.html` — Galaxian Clone**  
  Fixed-screen space shooter with dive attacks, score/lives HUD, and mobile control buttons.

- **`vaders.html` — Space Invaders**  
  Classic invader-defense gameplay with escalating pressure, synth-like SFX, and mobile controls.

- **`lander.html` — Lunar Lander**  
  Physics-flavored lander challenge where you manage angle, thrust, fuel, and descent speed to touch down safely.

- **`pacman.html` — Maze Muncher**  
  Pac-Man-style maze game with pellets, power orbs, and a ghost state machine (chase/frightened behavior).

- **`pool.html` — Emerald Pocket Pro (English Edition)**  
  Top-down pool/billiards simulation with cue drag aiming, adjustable shot power, and “english”/spin controls.

- **`pennyfalls.html` — Neon Penny Falls 3D**  
  3D coin-pusher style game using physics + WebGL rendering where you drop coins and try to maximize push outcomes.

### Simulators & interactive science/engineering demos

- **`NebularHypothesisSimulation.html` — Stellar Genesis (N-Body Accretion)**  
  A nebular hypothesis-inspired gravity simulation with tunable parameters (G, timestep, spin, friction) and orbital body formation.

- **`EntropyWordGenerator.html` — Entropy Word Generator**  
  Entropy-driven word generation utility for creating randomized word outputs/sequences.

- **`SparkGapSimulator.html` — Frankenstein Spark Gap Transmitter**  
  A stylized “mad-science” electrical apparatus sim featuring charge/spark behavior, dials/switches, and dramatic audiovisual feedback.

### Audio, speech, and ambient tools

- **`voicescribe.html` — VoxScribe (Advanced Speech-to-Text)**  
  Browser speech transcription utility with start/stop recording, editable transcript area, clipboard copy, and text download.

- **`chatter.html` — VoxScribe (Premium Speech + Conversation UI)**  
  Expanded speech interface with conversational transcript flow, settings persistence, and optional local AI model integration hooks.

- **`FrequencyDetector.html` — FreqHunter Quantum**  
  Real-time microphone spectrum/signal dashboard with analyzer visualizations and configurable signal-intelligence themed controls.

- **`sleep.html` — Lumen Slumber**  
  Ambient sensory relaxation aid combining generative visuals and audio controls designed for calming/focus/sleep routines.

- **`cuckooclock.html` — Chalet Cuckoo Clock / Chalet Automata**  
  Animated decorative clockwork experience with synchronized pendulum motion, cuckoo animation, and synthesized clock/chime-style audio.

## Relevant notes

- **Everything is self-contained**: each app is intentionally authored as a single HTML document for easy sharing and quick experimentation.
- **No framework build pipeline**: dependencies are mostly browser-native APIs plus CDN-hosted libraries in some files.
- **Microphone-dependent apps**: `voicescribe.html`, `chatter.html`, and `FrequencyDetector.html` require mic access and compatible browser APIs.
- **Potentially heavy rendering/physics apps**: `pennyfalls.html`, the stellar simulations, and some canvas-heavy games may perform better on desktop GPUs.
- **Local storage usage**: some apps (notably speech/chat variants) persist preferences (for example language/model settings) in `localStorage`.
- **Network expectations for some features**: several files load external assets/libraries from CDNs; offline execution may disable or degrade those features.
- **Variant naming/history**: there are two similarly themed stellar simulation files (`NebularHypothesisSimulation.html` and `EntropyWordGenerator.html`), and two VoxScribe-themed speech apps (`voicescribe.html` and `chatter.html`) with different scope/complexity.

## Verification snapshot (inspected April 6, 2026)

All HTML files in this repository were manually re-checked against this README index:

- `breakout.html`: ✅ description matches (levels, power-ups, keyboard/touch controls).
- `galaxians.html`: ✅ description matches (dive attacks, score/lives HUD, mobile controls).
- `vaders.html`: ✅ description matches (Space-Invaders-style loop, escalating pressure, mobile controls).
- `lander.html`: ✅ description matches (fuel/thrust/angle management with landing conditions).
- `pacman.html`: ✅ description matches (pellets + power pellets + frightened ghost state behavior).
- `pool.html`: ✅ description matches (drag aiming, power bar, cue spin/“english” controls).
- `pennyfalls.html`: ✅ description matches (3D coin pusher using WebGL + physics engine).
- `NebularHypothesisSimulation.html`: ✅ description matches (stellar accretion/gravity simulation with tunable parameters).
- `EntropyWordGenerator.html`: ✅ corrected above (entropy-based word generation tool).
- `SparkGapSimulator.html`: ✅ description matches (spark-gap apparatus sim with dials/switches and audiovisual feedback).
- `voicescribe.html`: ✅ description matches (speech-to-text with editable transcript, copy, and download).
- `chatter.html`: ✅ description matches (conversation-oriented VoxScribe variant with persistence and AI integration hooks).
- `FrequencyDetector.html`: ✅ description matches (real-time mic frequency/intel dashboard).
- `sleep.html`: ✅ description matches (ambient sensory sleep/focus aid).
- `cuckooclock.html`: ✅ description matches (animated cuckoo clock with synthesized clock/chime audio).

## Suggested future improvements

- Add a simple launcher/index page with thumbnails and tags (game, simulation, speech, audio).
- Normalize naming conventions (e.g., align file names with app titles).
- Add per-app mini docs (controls, browser support, known issues).
- Add license and attribution details for third-party libraries/assets.
