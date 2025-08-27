# Master’s Project Proposal — AI-Assisted Modernization of Legacy Game Soundtracks

**Student:** [Your Name]  
**Supervisor:** Dr. Fatemeh Jamshidi (Cal Poly Pomona)  
**Date:** [Insert Date]

## Title
AI-Assisted Modernization of Legacy Game Soundtracks: From Re-Orchestration to Generative Composition

## Motivation
Game music must adapt to interactive, non-linear experiences. Legacy soundtracks often use dated instrumentation and production. With Creative AI, we can modernize these works while preserving motifs; beyond that, compose new pieces inspired by the originals.

## Research Problem & Objectives
**RQ:** How can AI modernize legacy video game soundtracks while preserving stylistic integrity, and extend toward generating new music in the same style?

**Objectives:**
1) Build a modernization pipeline (symbolic analysis → re-orchestration → timbre transfer).  
2) Explore generative composition conditioned on motifs/chords.  
3) Evaluate with listener tests (MUSHRA) and objective metrics (FAD, motif retention).

## Methodology
**Phase A — Modernization**
- Data: MIDI or transcription of legacy cues (analysis-only).
- Analysis: key, chords, sections, leitmotifs.
- Re-orchestration: rules + ML suggestions.
- Timbre transfer: DDSP/neural synthesis; render stems, mix in DAW.

**Phase B — Generative Composition**
- Symbolic generation (Transformer) or audio-level model (MusicGen-like) with conditioning.
- Render & orchestrate with modern palette.

**Evaluation**
- Subjective: MUSHRA listening tests vs. original and human baseline.
- Objective: Fréchet Audio Distance to modern reference corpus; motif retention metrics.

## Deliverables
- Working pipeline & codebase, dataset inventory, demo tracks, evaluation report, paper-style write-up.

## Timeline
Semester 1: Phase A + eval v1.  
Semester 2: Phase B + full study + thesis.

## Licensing Note
Legacy OSTs retained for analysis only; training/testing on licensed or public-domain datasets.
