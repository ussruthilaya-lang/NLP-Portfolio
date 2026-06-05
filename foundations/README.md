# Foundations

Core building blocks of NLP, built from scratch in pure Python.
Everything here is a primitive. No shortcuts, no libraries.
These are the functions that every real NLP pipeline is built on top of.

---

## Progress Tracker

| Day | File | What I Built | What I Learned | Key Debug to Remember |
|-----|------|-------------|----------------|-----------------------|
| 1 | `day1_strings_tokenizer.py` | Tokenizer orchestrator — cleans raw text, builds a deduplicated vocabulary and maps every word to a unique index | Text cleaning via string manipulation, flattening and deduplicating vocab, indexing words into a dictionary | Always check the shape of your data at every function boundary, wrong shape going in means wrong or broken output coming out, and the same shape bug can cause multiple different errors downstream |
| Day | File | What I Built | What I Learned | Key Debug to Remember |
|-----|------|-------------|----------------|-----------------------|
| 1 | `day1_strings_tokenizer.ipynb` | Tokenizer orchestrator — cleans raw text, builds a deduplicated vocabulary and maps every word to a unique index | Text cleaning via string manipulation, flattening and deduplicating vocab, indexing words into a dictionary — this is the preprocessing foundation of every real NLP pipeline | Always check the shape of your data at every function boundary — wrong shape going in means wrong or broken output coming out, and the same shape bug can cause multiple different errors downstream |
| 2 | `day2_bow_vectors.ipynb` | Bag of Words vectorizer - converts each sentence into a numeric vector by marking vocab word positions as 1, everything else 0 | A sentence becomes a fixed-length vector one slot per vocab word not per sentence word. This is the mathematical fingerprint of text that models learn from. Core limitation: large vocab = huge sparse vectors, mostly 0s this is why Word2Vec and BERT were invented | Always initialise vector as `[0] * len(word_to_index)` and iterate vocab slots not sentence words also `()` is a generator `[]` is a list, always use `[]` |