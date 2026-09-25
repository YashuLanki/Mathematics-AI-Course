# NLP Document Similarity

AIT 525 assignment — measuring similarity between two documents using NLP.

Preprocesses two NLP research papers — ["Attention Is All You Need"](https://arxiv.org/abs/1706.03762) and ["BERT"](https://arxiv.org/abs/1810.04805), the second built directly on the first's Transformer architecture — and vectorizes them using Bag of Words and TF-IDF, then compares the results using cosine similarity to evaluate how well each technique captures document similarity.

- [`nlp.ipynb`](./nlp.ipynb) — the full notebook: preprocessing, BoW/TF-IDF vectorization, cosine similarity, and evaluation.
- [`nlp_data/`](./nlp_data) — the two source papers as PDFs (see its README for sources).
- `NLP_Assignment.docx` — original assignment instructions (not tracked in git).
- `script.md` — narration script for the video presentation (not tracked in git).
