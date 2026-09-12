# Video Presentation Script

**Target length: ~3:45–4:00**

---

## Intro (~15s)

Hi, I'm Yashu Lanki, and this is my presentation for AIT 525 — predicting fish weight using linear regression. I used a dataset of 158 fish across seven species, with five physical measurements as predictors: three length measurements, height, and width.

---

## The Algorithm (~50s)
*[Screencast: Section 3 — Mathematical Model Design]*

The core idea behind linear regression is that weight can be predicted as a weighted sum of these five measurements, plus a baseline intercept. Each coefficient tells you how much predicted weight changes for a one-unit increase in that feature, holding the others constant.

To find the best coefficients, the model minimizes a cost function — mean squared error, or the average squared difference between predicted and actual weight. There are two ways to minimize that cost function: a closed-form solution that solves for the coefficients directly in one step, and gradient descent, which starts with a guess and iteratively nudges the coefficients in the direction that reduces error, until it converges. I implemented both, so I could compare them directly.

---

## Code Demonstration (~70s)
*[Screencast: Section 2 — Dataset Exploration, then Section 4 — Model Implementation]*

Before modeling, I explored the data and found one fish with a recorded weight of zero grams — which isn't biologically possible — so I removed that row. I also checked for negative measurements and confirmed there weren't any.

For the baseline model, I split the data into training and test sets, then fit a standard linear regression model using scikit-learn's closed-form solver. That gives me a first set of predictions.

For the optimized version, I used gradient descent instead — specifically, scikit-learn's SGDRegressor. Since gradient descent is sensitive to feature scale, I standardized all five measurements first, then fit the model iteratively on the scaled training data. Both models generate predictions on the same held-out test set, so the comparison is apples-to-apples.

---

## Performance Comparison (~50s)
*[Screencast: Section 5 — Performance Evaluation]*

Comparing the two: the baseline model had a mean squared error of about 12,829, which works out to a typical prediction error of roughly 113 grams, and an R-squared of 0.904 — meaning it explains about 90% of the variance in fish weight. The gradient descent model was very close behind, with an R-squared of 0.897 and a typical error around 118 grams.

That small gap is actually a meaningful result — it confirms gradient descent successfully approximates the same underlying relationship that the closed-form method solves for exactly. In practice, this matters because closed-form solutions don't scale well to very large datasets, while gradient descent does — so knowing it gets nearly identical results here validates using it on bigger problems.

---

## Real-World Applications (~50s)
*[Screencast: Section 6 — Real-World Applications]*

Regression like this generalizes well beyond fish. In resource allocation, businesses predict staffing or inventory needs from easy-to-measure signals like order volume or seasonality. In customer retention, companies predict churn risk from usage patterns, so they can prioritize outreach to the customers most likely to leave. And in demand forecasting, regression predicts future sales from price, advertising spend, and market indicators — helping companies make informed, proactive decisions instead of reacting after the fact.

The common thread is the same one from this project: when the input features are cheap to measure but the outcome you care about isn't, regression lets you predict it anyway.

---

## Close (~10s)

To summarize: a simple five-feature linear model explained about 90% of the variation in fish weight, and both the closed-form and gradient descent approaches produced nearly identical, reliable results. Thanks for watching.
