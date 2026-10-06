# Dataset: r/MachineLearning Reply Network (2014)

User-interaction network for the r/MachineLearning subreddit, taken from Stanford SNAP's [Reddit user interaction networks](https://snap.stanford.edu/data/web-RedditNetworks.html) collection (the `reddit_reply_networks` archive).

- **Nodes:** Reddit users who commented at least 50 times during 2014.
- **Edges:** directed replies — an edge from user A to user B means A replied directly to B's comment.
- **Time:** 11 monthly networks (2014, holiday period excluded), roughly 270–430 users and 340–660 reply edges per month, 2,150 unique users overall.

## File

- `MachineLearning.json` — a JSON list of 11 monthly networks. Each month is an adjacency list: `{"username": ["user_they_replied_to", ...], ...}`.

## Citation

Hamilton, W. L., Zhang, J., Danescu-Niculescu-Mizil, C., Jurafsky, D., & Leskovec, J. (2017). Loyalty in online communities. *Proceedings of the International AAAI Conference on Web and Social Media*, *11*(1), 540–543.
