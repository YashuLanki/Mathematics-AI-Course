# Bayes' Theorem: How AI Learns to Spot Spam

AIT 525 final assignment — a video presentation on Bayes' theorem in AI, covering Christian values in responsible AI, the math behind Bayes' theorem, the Naive Bayes spam filter as an AI application, and its free market impact.

Applies Bayes' theorem to the SMS Spam Collection (5,574 text messages, 13.4% spam). By hand, the word "free" raises the chance a message is spam from 13.4% to 74.2%. A multinomial Naive Bayes classifier trains in about 1 ms and scores 98.5% test accuracy, wrongly flagging only 3 of 966 legitimate messages, and its word likelihood ratios show why each message is flagged.

- [`bayes_spam.ipynb`](./bayes_spam.ipynb) — the notebook behind the presentation's numbers: Bayes' theorem by hand for one word, the Naive Bayes classifier and its metrics, and a word likelihood-ratio chart.
- [`sms_data/`](./sms_data) — the SMS Spam Collection dataset (UCI Machine Learning Repository) and its readme.
- [`Bayes_Spam_Filter.pptx`](./Bayes_Spam_Filter.pptx) — the 12-slide presentation deck, with the narration in each slide's speaker notes.
- `Final_Assignment.docx` — original assignment instructions (not tracked in git).
- `script.md` — narration script for the video presentation (not tracked in git).
