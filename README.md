# Sylva

A browser-based ambient forest environment for nervous system regulation, using passive bilateral visual stimulation, breath entrainment, and layered nature audio — no instructions, no compliance required.

---

## What it is

Sylva is a single-file web application that renders a generative NZ native forest (ngahere). Birds cross the screen from side to side, carrying the eye with them in a slow bilateral movement. Wind moves through the trees on a spring-mass physics system. A low drone, pink noise wind, and stream layer build a passive audio environment. A breath cycle modulates light, sound, and motion at ~5 breaths per minute — the HRV resonance frequency shown to maximise parasympathetic tone.

The forest does the work. There is nothing to do, follow, or complete.

---

## Theoretical basis

Sylva draws on Francine Shapiro's observation that walking through a forest produced the natural bilateral eye movement that led to the development of EMDR. Rather than abstracting bilateral stimulation into a clinical dot, Sylva embeds it in its ecological origin — the passing of birds through a forest canopy.

The three regulatory mechanisms operate passively and simultaneously:

- **Bilateral visual stimulation** — birds cross the full screen width at speeds calibrated to the clinically studied 0.8–1.2 Hz EMDR range (Focus mode) or slower meditative tracking (Settle mode)
- **Breath entrainment** — a 12-second breath cycle (~5 bpm) modulates ambient light, drone pitch, and wind volume, within the resonance frequency shown to maximise HRV
- **Nature audio** — layered wind, stream, and drone sounds draw on research showing forest soundscapes measurably reduce sympathetic nervous activity, heart rate, and tension-anxiety

---

## Technical

- Single HTML file, no dependencies, no build step
- Web Audio API — triangle wave drone, pink noise wind and stream layers, shimmer
- Spring-mass wind physics — non-periodic, depth-scaled across three parallax layers
- Device-independent bird timing — crossing speed calculated in wall-clock milliseconds, correct at 60 Hz, 120 Hz, or any framerate
- Works on desktop, tablet, and mobile
```bash

---

## Modes

| Mode | Bird speed | Use |
|------|-----------|-----|
| Settle | 7–11s per crossing | General regulation, rest, deactivation |
| Focus | 1.8–2.8s per crossing | Active attention tracking, closer to clinical BLS |

Sound levels: Off / Soft / Full. Visual display can be hidden (Listen mode) to use as audio-only.

---

## Status

Single-file prototype. Actively tested with users. What remains empirically open: whether passive ambient delivery of bilateral stimulation and breath entrainment produces measurable regulation effects without conscious compliance or instruction.

---
