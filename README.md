# Apex Chess & Checkers AI

**Play Live:** https://tawankung000.github.io/chess-bot-checkers-bot/

An interactive, single-file **Chess & Checkers** web game powered by a custom in-browser tactical AI engine, real-time 7-tier move analysis, tournament clocks, playable variants, and living animated piece skins. Runs directly in any desktop or mobile browser with zero dependencies.

---

## Features

### Smart AI Engine & Play Modes
- **Apex Chess AI:** Iterative-deepening Principal Variation Search (Alpha-Beta), Zobrist transposition tables, quiescence search, Late Move Reductions, null-move pruning, PeSTO tapered evaluation, and a Grandmaster opening book running inside a Web Worker.
- **Apex Checkers AI:** Dedicated 8x8 American Checkers search engine with mandatory jump chains, jump-quiescence search, automatic King crowning, and endgame King-chase evaluation.
- **3 Bot Difficulty Tiers:** **Club (1600)**, **Master (2100)**, and **Apex GM (2550 Max)**.
- **Pass & Play (2-Player Local):** Play Chess (any variant) or Checkers against a friend on the same device.

### 7-Tier Real-Time Move Analysis
- Evaluates every move using win-probability shifts and tactical sacrifice checks:
  - **Brilliant (`!!`)** — Sound tactical piece sacrifices with a diamond-cyan shockwave burst
  - **Book (`Book`)** — Standard Grandmaster opening theory
  - **Best (`Best`)** — Engine's top choice with a powerful golden-emerald slam animation
  - **Good (`Good`)** — Accurate, solid continuation
  - **Inaccuracy (`?!`)** — Minor positional or tactical slip
  - **Mistake (`?`)** — Clear error with Best Move arrow guidance
  - **Blunder (`??`)** — Major oversight with an unsure recoil-and-wobble animation
- **Interactive Replay:** Click any move in the Move History table or use the `Prev` / `Next` / `Live` controls (and Left/Right arrow keys) to inspect positions and view engine Principal Variation lines.

### Chess Clocks & Time Controls
- **5 Modes:** `Off` (Unlimited), `1 min` (Bullet), `3 | 2` (Blitz with +2s increment), `5 min` (Blitz), and `10 min` (Rapid).
- **Precision Readout:** Tenths-of-a-second display under 10 seconds, low-time pulse warnings, countdown ticks, and automatic AI speed-up under time pressure.

### Playable Chess Variants
- **Standard:** Classic FIDE tournament rules.
- **Chaos 960:** Shuffled symmetrical back-rank setups with opposite-colored bishops for pure calculation from move 1.
- **Atomic:** Captures detonate a 3x3 fireball explosion destroying surrounding non-pawn pieces—win instantly by detonating the enemy King.
- **Knightmare:** 6 Knights + Queen + King per side for nonstop cavalry forks.

### Living Skins, Expressive Bot & Polish
- **5 Live-Switchable Skins:** **Classic**, **Cyber Neon**, **Royal Gold**, **Googly**, and **Cats & Dogs** (supporting both Chess pieces and Checkers discs/kings).
- **Living Board Physics:** Real-time cursor-tracking eyes, spontaneous blinking, high-hover pickup levitation, momentum drag-tilt banking, cowering capture targets, and King-in-check panic shivers.
- **Expressive Apex Bot:** Mood-reactive animated bot avatar (click its face to poke it!) paired with typewriter commentary and synthesized Web Audio sound effects.
- **Responsive & Dark Mode:** Dynamic `100dvh` viewport scaling for 100% browser zoom on laptops/desktops, elevated mobile touch-drag previews, and instant Light/Dark Mode switching.

---

## Changelog

### v1.3.0
- **Live Interactive Momentum Graph:** Real-time SVG evaluation curve in Move Analysis showing White/Black advantage per ply, highlighting `!!`, `?`, and `??` moves with click-to-jump board navigation.
- **Post-Game Accuracy Report Card:** Auto-opening post-game modal (reopenable via the Move Analysis **Review** button) featuring 0–100% Overall Accuracy, Estimated Performance Elo, a 7-tier Move Breakdown, and a **Turning Point** jump button.
- **Bot Personalities & Boss Fight Rivals:** 5 selectable rivals—Trash-Talk Goblin (1500), Sleepy Cat Master (1900), Apex Bot (2100), Polite Grandmaster (2550), and Cyber Overlord (BOSS MAX, 18-ply)—complete with animated SVG faces, cursor-tracking eyes, Web Audio voices, distinct playstyles, and reactive typewriter dialogue.

### v1.2.0 — Chess Clocks & Brilliant (`!!`) Moves (Latest)
- **Added:** Inline digital chess clocks on both player cards with tenths-of-a-second precision below 10 seconds and final-10-second audio ticks.
- **Added:** 5 time control presets (`Off`, `1 min`, `3 | 2`, `5 min`, `10 min`), time-pressure speed scaling for Apex Bot, and timeout / bare-king draw rules.
- **Added:** **Brilliant (`!!`)** move rank for sound tactical sacrifices in both Chess and Checkers, complete with diamond-cyan burst FX, crystalline arpeggio audio, and shocked Bot reactions.

### v1.1.0 — Checkers, Variants, Living Skins & Expressive Bot
- **Added:** Full playable **American Checkers (8x8)** mode with dedicated AI and multi-jump hop animations.
- **Added:** **Pass & Play (2P Local)** mode, **Dark Mode** toggle, and mobile touch-drag layout enhancements.
- **Added:** Playable **Chaos 960**, **Atomic**, and **Knightmare** chess variants.
- **Added:** 5 live-switchable skins (**Classic**, **Cyber Neon**, **Royal Gold**, **Googly**, **Cats & Dogs**) with real-time cursor-tracking eyes, blinking, and high-levitation pickup tilt physics.
- **Added:** Animated **Apex Bot** face with mood expressions and live typewriter speech bubble.
- **Fixed:** Dynamic viewport board scaling (`100dvh`) so the bot face, full 8x8 board, and player bar fit simultaneously at 100% desktop browser zoom.

### v1.0.0 — Initial Launch
- **Added:** Core **Apex Chess AI** Web Worker engine (Alpha-Beta PVS, Zobrist TT, PeSTO tapered evaluation, and GM opening book).
- **Added:** Complete FIDE chess rules, real-time Move Analysis with Principal Variation lines, Undo Move, Flip Board, and procedural Web Audio sound effects.

---

## Running Locally
No build tools or installation required—download `index.html` and open it directly in any modern browser (Chrome, Edge, Firefox, or Safari).
