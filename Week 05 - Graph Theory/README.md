# Graph Theory and Social Influence Prediction

AIT 525 assignment — modeling a social network as a graph and predicting social influence.

Builds a user-interaction graph from the r/MachineLearning reply network ([Stanford SNAP](https://snap.stanford.edu/data/web-RedditNetworks.html), 2014) with NetworkX — 299 users as nodes, 411 replies as directed edges — then runs random walks and computes degree and betweenness centrality to score each user's social influence. A logistic regression combines friends' activity with those influence scores to predict whether each user stays active the next month, evaluated with AUC (0.66, vs. 0.58 using friends' activity alone). The notebook closes with a discussion of the ethics of graph-based influence prediction.

- [`graph_theory.ipynb`](./graph_theory.ipynb) — the full notebook: graph construction and visualization, random walks and influence scoring, the prediction algorithm with AUC evaluation, and ethical considerations.
- [`reddit_data/`](./reddit_data) — the r/MachineLearning reply network (see its README for source and format).
- `graph_theory_assignment.docx` — original assignment instructions (not tracked in git).
- `script.md` — narration script for the video presentation (not tracked in git).
