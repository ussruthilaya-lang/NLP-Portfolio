# Foundations

Core building blocks of NLP, built from scratch in pure Python.
Everything here is a primitive. No shortcuts, no libraries.
These are the functions that every real NLP pipeline is built on top of.

---

## Progress Tracker

| Day | File | What I Built | What I Learned | Key Debug to Remember |
|-----|------|-------------|----------------|-----------------------|
| 1 | `day1_strings_tokenizer.py` | Tokenizer orchestrator — cleans raw text, builds a deduplicated vocabulary and maps every word to a unique index | Text cleaning via string manipulation, flattening and deduplicating vocab, indexing words into a dictionary | Always check the shape of your data at every function boundary, wrong shape going in means wrong or broken output coming out, and the same shape bug can cause multiple different errors downstream |