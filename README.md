# NLP Portfolio — Built From Scratch

A hands-on journey building NLP systems from the ground up.
No ML libraries. Pure Python + NumPy + Pandas.
Every model is hand-coded, every concept is understood before it is written.

## Goal
Transition from data analyst to AI engineer with deep NLP foundations.
Focus areas: Healthcare NLP → Finance → Enterprise AI systems.

## Philosophy
- Understand the math first, then write the code
- No black boxes - every line is explainable
- Real datasets, not toy examples
- Daily commits - code goes up every day

---

## Progress Tracker

| Day | File | What I Built | What I Learned | Key Debug to Remember |
|-----|------|-------------|----------------|-----------------------|
| 1 | `foundations/day1_strings_tokenizer.py` | Tokenizer orchestrator - a pipeline that cleans raw text, builds a deduplicated vocabulary and maps every word to a unique index | Text cleaning via string manipulation, flattening and deduplicating vocab, indexing words into a dictionary this is the preprocessing foundation of every real NLP pipeline | Always check the shape of your data at every function boundary wrong shape going in means wrong or broken output coming out, and the same shape bug can cause multiple different errors downstream |

---

## Repo Structure

\```
NLP-Portfolio/
├── foundations/       # core Python + NLP building blocks
├── models/            # ML models built from scratch
├── projects/          # real dataset pipelines
└── README.md
\```