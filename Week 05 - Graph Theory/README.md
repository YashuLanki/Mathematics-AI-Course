# Graph Theory and Social Influence Prediction

AIT 525 assignment — modeling a social network as a graph and predicting social influence.

Builds a user-interaction graph from the r/MachineLearning reply network ([Stanford SNAP](https://snap.stanford.edu/data/web-RedditNetworks.html), 2014) with NetworkX, runs random walks and centrality measures to score each user's social influence, then develops and evaluates an algorithm that predicts user actions from those influence scores.

- [`graph_theory.ipynb`](./graph_theory.ipynb) — the full notebook: graph construction, random walks and influence scoring, and the prediction algorithm with evaluation.
- [`reddit_data/`](./reddit_data) — the r/MachineLearning reply network (see its README for source and format).
- `graph_theory_assignment.docx` — original assignment instructions (not tracked in git).
- `script.md` — narration script for the video presentation (not tracked in git).
