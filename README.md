# Sylva

A browser-based ambient forest environment for nervous system regulation, using passive bilateral visual stimulation, breath entrainment, and layered nature audio — no instructions, no compliance required.

---

## What it is

Sylva is a single-file web application that renders a generative NZ native forest (ngahere). Birds cross the screen from side to side, carrying the eye with them in a continuous bilateral movement. Wind moves through the trees on a spring-mass physics system. A low drone, pink noise wind, and stream layer build a passive audio environment. A breath cycle modulates light, sound, and motion at ~5 breaths per minute — the HRV resonance frequency shown to maximise parasympathetic tone.

The forest does the work. There is nothing to do, follow, or complete.

---

## Theoretical basis

Sylva draws on Francine Shapiro's observation that walking through a forest produced the natural bilateral eye movement that led to the development of EMDR. Rather than abstracting bilateral stimulation into a clinical dot, Sylva embeds it in its ecological origin — the passing of birds through a forest canopy.

The three regulatory mechanisms operate passively and simultaneously:

- **Bilateral visual stimulation** — birds cross the full screen width at speeds calibrated to engage smooth pursuit tracking. Ease mode supports gentle orienting; Deep mode approaches the lower range of clinically studied BLS frequencies.
- **Breath entrainment** — a 12-second breath cycle (~5 bpm) modulates ambient light, drone pitch, and wind volume, within the resonance frequency shown to maximise HRV.
- **Nature audio** — layered wind, stream, and drone sounds draw on research showing forest soundscapes measurably reduce sympathetic nervous activity, heart rate, and tension-anxiety.

---

## Technical

- Single HTML file, no dependencies, no build step
- Web Audio API — triangle wave drone with autonomous pitch drift, pink noise wind and stream layers
- Spring-mass wind physics — non-periodic, depth-scaled across three parallax layers
- Device-independent bird timing — crossing speed in wall-clock milliseconds (`pxPerMs * dt`), correct at 60 Hz, 120 Hz, or any framerate
- Progress-based spawn scheduling — next bird spawns at a fixed traversal threshold, not a timer, eliminating gaps across all screen sizes and frame rates
- Works on desktop, tablet, and mobile

---

## Modes

| Mode | Crossing duration | Feel |
|------|------------------|------|
| Ease | 2.5–4.0s per crossing | Gentle orienting; easy continuous tracking |
| Deep | 1.0–1.6s per crossing | More directive rhythm; stronger entrainment |

Audio levels and wind intensity are baked into each mode preset — Ease is quieter and stiller, Deep is louder and more present.

---

## Status

Single-file prototype. Actively tested with users. What remains empirically open: whether passive ambient delivery of bilateral stimulation and breath entrainment produces measurable regulation effects without conscious compliance or instruction.

---

## Credits

Developed by Superfutures Research. Concept rooted in the forest as a therapeutic environment in its own right.
