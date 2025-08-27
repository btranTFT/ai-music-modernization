# AI-Assisted Modernization of Legacy Game Soundtracks

**Student:** _Your Name_  
**Supervisor:** Dr. Fatemeh Jamshidi (Cal Poly Pomona)  
**Created:** 2025-08-27

## Overview
This repository contains a two-phase research project:
- **Phase A (Modernization):** Transcribe/ingest legacy cues → analyze motifs/harmony → re-orchestrate with a modern palette → timbre transfer & rendering.
- **Phase B (Generative Composition):** Train or condition models to compose new music *in the style*, guided by motifs/chords from Phase A.

## Repo Layout
```
data/               # datasets (untracked audio by default)
docs/               # papers, proposal, diagrams
notebooks/          # exploratory notebooks
scripts/            # CLI utilities
src/                # python packages for each pipeline stage
experiments/        # configs & runs
results/            # audio and figures
integration/        # FMOD/Wwise prototypes
```

## Quickstart
```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
```

## Pipelines
- `src/transcription/`: MIDI extraction & alignment (BasicPitch/Onsets&Frames).
- `src/analysis/`: motif detection, chord/key/structure (music21, librosa).
- `src/orchestration/`: rule-based & learned mappings legacy→modern instruments.
- `src/timbre_transfer/`: DDSP models for neural re-voicing and rendering.
- `src/generation/`: symbolic and audio-level generation (Transformers, MusicGen-like).
- `src/evaluation/`: MUSHRA harness, Fréchet Audio Distance (FAD), motif retention metrics.

## Ethics & Licensing
- Treat copyrighted OSTs as **analysis-only**; train on **licensed or public-domain** data.
- Maintain a `DATA_SOURCES.md` inventory noting license for each dataset and how it is used.
- Keep human-in-the-loop edits documented (for authorship & reproducibility).

## Milestones
- **M1:** Transcription+analysis baseline (Week 4)
- **M2:** Phase A modernization demo (Week 8)
- **M3:** Evaluation v1 (Week 10)
- **M4:** Phase B generation demo (Week 12+)
- **M5:** Final study & write-up (End of term)

## Contacts
- Supervisor: Dr. Fatemeh Jamshidi
- Student: Your Name
