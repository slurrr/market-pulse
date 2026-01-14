# Market Pulse — Throwaway Experiment

This repository is a **throwaway-first experiment** to build a real-time crypto **market pulse dashboard**.

It is not a scanner, not a signal engine, not a trading system, and not a long-term codebase.

The goal is to collapse inference from many disparate data sources into a single situational awareness view that helps a human trader understand **what the market is doing right now**.

This repo is expected to be deleted.

---

## How to Work in This Repo (Read This First)

1. **Read `vision.md` before doing anything else**
   - It defines intent, constraints, and non-goals.
   - The question list is inspiration, not a requirements checklist.

2. **Optimize for usefulness now**
   - Correctness, elegance, and architecture are secondary.
   - False positives are costly. Silence is acceptable.

3. **You are free to invent structure**
   - No frozen architecture.
   - No frozen interfaces.
   - No premature invariants.
   - If something hurts to change, change it anyway.

4. **Prefer implementation over discussion**
   - If unsure, build it and observe.
   - Visuals > abstractions.
   - Ratios, comparisons, and deltas > raw numbers.

5. **Delete aggressively**
   - If something does not improve situational awareness, remove it.
   - Deletion is progress.

---

## Source Control Philosophy

Use Git as a **scratchpad**, not a guardrail.

- Commit early and often.
- Small, messy commits are fine.
- Breaking things is fine.
- Rewriting history is fine.
- Deleting large sections of code is encouraged.

Do not:
- Preserve code “just in case”
- Avoid changes because of git history
- Treat commits as permanent decisions

If something feels wrong, delete it and move on.
Git exists so you can be fearless.

---

## Work Modes

This project operates in explicit modes.

### ADDITIVE MODE (default)
- Add new dimensions, lenses, or panels
- Do not remove existing ones unless they are clearly broken
- Depth is less important than breadth
- Redundancy is acceptable

### REDUCTION MODE (invoked explicitly)
- Delete, merge, or collapse existing elements
- No new features
- Prefer calmness and legibility

### AUDIT MODE (invoked explicitly)
- No code changes
- Assess feel, language, and usefulness only
- Write observations, not fixes

If a mode is not specified, assume ADDITIVE MODE.

---

## Artifact Discipline (Critical)

Artifacts exist to preserve **learning**, not structure.

When you make a meaningful decision, discovery, or observation, write it down.

Use these files only when needed:

- `decisions.md`
  - Append-only
  - Why a choice was made, not how it was implemented

- `dashboard_notes.md`
  - What feels useful, misleading, noisy, or surprising
  - Human-facing observations

- `data_sources.md`
  - What data feeds actually mattered in practice

- `candidate_invariants.md`
  - Patterns that *keep reappearing*
  - Observational only — **do not enforce**

Do **not** create:
- task lists
- roadmaps
- architecture diagrams
- specs
- long plans

---

## Session Reset Rules

At the start of a new session:

1. Read:
   - `vision.md`
   - `README.md`
   - `decisions.md` (if it exists)

2. State briefly (1 paragraph):
   - Your understanding of the project
   - What you are about to work on

3. Load **only** the context needed for the current task.

---

## Ground Rules

- This is an observational dashboard, not a prescriptive system.
- Showing tension, imbalance, and disagreement is va
