# Models

ML models built from scratch — pure Python + NumPy.
No sklearn, no torch. Every algorithm is hand-coded with full understanding of the math.
Each model builds on the preprocessing primitives in `foundations/`.

---

## Progress Tracker

| Day | File | What I Built | What I Learned | Key Debug to Remember |
|-----|------|-------------|----------------|-----------------------|
| 3 | `naive_bayes/day3_naive_bayes.py` | Naive Bayes classifier - calculates class probabilities and per word probabilities per class, uses them to predict if a new comment is toxic or not | Laplace smoothing handles unseen words by adding 1 to every word count so no probability is ever zero. Log probabilities prevent underflow — multiplying many small decimals together eventually rounds to zero, addition of logs never does | Never access a dictionary directly with `dict[word]` during prediction — always use `.get(word, fallback)`. `if/else` must always be inside the `for` loop not attached to it. Reusing loop variable names in nested loops overwrites the outer variable silently |