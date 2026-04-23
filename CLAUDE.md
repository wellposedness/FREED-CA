# FREED-CA — Claude Code Context

**FREED-CA** = The Game of Truth — CA progression archive  
**Author**: David Harry Freed, mail carrier, Olney Maryland  
**Repo**: wellposedness/FREED-CA (GitHub Pages at wellposedness.github.io/FREED-CA/)

This repository is **completely isolated from the FREED daemon**. The daemon has no knowledge of this repo, no path to it, and no write access. All files here are hand-edited only.

---

## Purpose

Archive of every meaningful iteration of "The Game of Truth" — a cellular automaton built from first principles:
- Physics engine: Mandelbrot set (escape bands as energy zones)
- Agent types: cognitive taxonomy derived from RSA framework
- Question: what survives at the boundary between order and chaos?

---

## Files

```
index.html      — Gallery landing page. Shows all 11 versions with descriptions.
v1.html         — RSA-Omega: First Contact (gen 117)
v2.html         — The Aesthetic (gen 126)
v3.html         — Mandelbrot Physics (gen 133)
v4.html         — Zoom Trajectory (gen 134)
v5.html         — Alien Anatomical Layout (gen 140, reverted experiment)
v6.html         — Voronoi Foam Topology (gen 140)
v7.html         — 3-Panel HUD (gen 140)
v8.html         — Three Cognitive Types + Zipf (gen 141)
v9.html         — Variable Population (gen 141)
v10.html        — The Game of Truth — Six Types (gen 141)
v11.html        — Collective Memory (gen 148, current)
```

## Current simulation state (v11 — Collective Memory)

Inherits all v10 mechanics plus three additions:

**Aperiodic Mandelbrot shocks**: `aperiodicNoise(t) = (sin(0.019t)+sin(0.027t)+sin(0.048t))/3`. Fires when crossing 0.65, 80-step cooldown. Cycles through 6 boundary targets. Incommensurable frequencies → never periodic.

**Drifting resource hotspots**: 6 hotspots, 90px radius, +2.0 peak energy/step, 0.25px/step drift, slow phase oscillation. Energy landscape is quasi-stable, not uniform.

**Mortality tracking**: `perturbPending = {step, aliveBefore}`, measured 25 steps later. `mortalityHistory[]` stores rate per shock. Bar chart canvas (`#mort-canvas`) with red→green bars and linear regression trend line. Stats: perturbCount, last shock mortality %, trend (adapting/degrading/stable).

**Scientific claim**: Populations store information about past environments in their type distribution, producing measurable collective memory — without individual cells having memory. Mortality trend should decrease as type composition adapts.

## v10 simulation state (archived)

**Two axes**: loop depth (Builder/Navigator/Drifter) × grounding (Physics/Symbol).  
`type = depth*2 + grounding` (0–5). Six types:

| Type | Code | Color | Behavior |
|------|------|-------|----------|
| Physics Builder | 0 | cyan | Full RSA loop vs territory |
| Symbol Builder | 1 | violet | Full loop vs lagged map |
| Physics Navigator | 2 | green | 3-neighbor prediction vs territory |
| Symbol Navigator | 3 | amber | 3-neighbor prediction vs map |
| Physics Drifter | 4 | orange | Pure noise |
| Symbol Drifter | 5 | rose | Pure noise + divergence tax |

Symbol grounding mechanics: `SYMBOL_LAG = 0.65`, `GROUND_TAX = 2.5`.  
Mandelbrot zooms toward c=−0.75+0.1i. 7 escape bands. `ZOOM_PER_STEP = 0.995`.

**Key result**: Symbol Builders go nearly extinct at high Mandelbrot complexity. This is a falsifiable prediction of the Noether's Table, confirmed by the simulation.

---

## Rules

1. **Never add the Lorenz attractor** — not part of Dave's first-principles framework.
2. **Never add daemon status, sweep results, or any FREED live data** — this site is static.
3. **New CA versions go here** — add as `v11.html`, `v12.html`, etc. and update `index.html`.
4. **Reduce cell count if needed** — smooth performance matters more than density. Current Voronoi versions use N_CELLS=220 which is comfortable.
5. **This is not a RAG system, not a knowledge base** — it is a simulation archive.

---

## Adding a new version

1. Build the CA in `v11.html` (copy v10.html as a starting point)
2. Add the nav injection: copy the `<style id="ca-nav-style">` and `<div id="ca-nav">` pattern from any existing version
3. Add a card to `index.html`
4. Commit and push — no daemon, no CI, no build step needed

---

## What this is not

This repo has no daemon, no sweep, no L7, no obligations. It is a gallery of hand-crafted simulations. The connection to FREED is conceptual (the physics derives from Freed's Law) and navigational (FREED's index.html links here).
