# Eval Harness

Everything needed to answer one question: **did this change make the product better, or just different?**

## Contents

- `datasets/` — small, hand-labelled test sets built from real user inputs (20–50 cases beat 2,000 synthetic ones)
- `rubrics/` — what “good” means per task, written before the prompt
- `runs/` — dated result files, one per prompt/model version
- `scripts/` — harness code

## What every run records

| Field | Why |
| --- | --- |
| prompt version | ties result to a diff |
| model + version | models silently change |
| pass rate per rubric item | shows *where* it got worse |
| p50 / p95 latency | UX, not vanity |
| cost per 1k calls | product viability |

## Rule

A prompt change ships only with a run in `runs/` comparing old vs new. No run, no ship.
