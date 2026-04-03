# Sylva
A browser-based ambient forest environment for nervous system regulation, using passive bilateral visual stimulation, breath entrainment, and layered nature audio — no instructions, no compliance required.

---

## What it is
Sylva is a single-file web application that renders a generative NZ native forest (ngahere). A single bird crosses the screen from side to side, carrying the eye in a continuous bilateral movement. Wind moves through the trees on a spring-mass physics system. A low drone, pink noise wind, and stream layer build a passive audio environment. A breath cycle modulates light, sound, and motion at ~5 breaths per minute — the HRV resonance frequency shown to maximise parasympathetic tone.

The forest does the work. There is nothing to do, follow, or complete.

---

## Theoretical basis
Sylva draws on Francine Shapiro's observation that walking through a forest produced the natural bilateral eye movement that led to the development of EMDR. Rather than abstracting bilateral stimulation into a clinical dot, Sylva embeds it in its ecological origin — the passing of a bird through a forest canopy.

The three regulatory mechanisms operate passively and simultaneously:

- **Bilateral visual stimulation** — a single bird crosses the full screen width on each pass, alternating direction. Speed is derived from the breath cycle: one crossing per half-cycle in Ease mode, one per quarter-cycle in Deep mode. This phase-couples the tracking signal to the breath rhythm rather than running two independent timing systems.
- **Breath entrainment** — a 12-second cycle (~5 bpm) modulates ambient light, drone pitch, and wind volume within the resonance frequency shown to maximise HRV coherence.
- **Nature audio** — layered wind, stream, and continuous drone draw on research showing forest soundscapes measurably reduce sympathetic nervous activity, heart rate, and tension-anxiety.

---

## Technical

- Single HTML file, no dependencies, no build step
- Web Audio API — triangle wave drone with autonomous pitch drift, pink noise wind and stream layers
- Spring-mass wind physics — non-periodic, depth-scaled across three parallax layers
- Device-independent bird timing — crossing speed in wall-clock milliseconds, correct at 60 Hz, 120 Hz, or any framerate
- Singular bird model — exactly one bird active at all times, no overlap, no perceptible gap between passes
- Bird speed derived from breath cycle — traversal time is a direct function of `sCycleMs`, coupling visual and respiratory rhythms
- Unified state transitions — mode changes defer to the next spawn boundary, so bird speed and audio shift as a single field rather than independent parameters
- Continuous audio only — no event-based sound triggers; all layers are ongoing
- Works on desktop, tablet, and mobile

---

## Modes

| Mode | Crossing duration | Relationship to breath |
|------|------------------|----------------------|
| Ease | 3.5–7s per crossing | One crossing per half breath cycle |
| Deep | 1.5–3.5s per crossing | One crossing per quarter breath cycle |

Ease is suited to general regulation, rest, and deactivation. Deep produces faster bilateral passes closer to the clinically studied EMDR range.

---

## Status
Single-file prototype. Actively tested with users. What remains empirically open: whether passive ambient delivery of bilateral stimulation and breath entrainment produces measurable regulation effects without conscious compliance or instruction.
