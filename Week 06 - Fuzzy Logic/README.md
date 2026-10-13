# Fuzzy Logic Fuel Economy Prediction for a Toyota Tundra

AIT 525 assignment — designing and implementing a fuzzy logic system for a real-world decision problem with uncertain or imprecise inputs.

Builds a Mamdani fuzzy logic system with scikit-fuzzy that predicts a Toyota Tundra's fuel economy (MPG) from cargo load (0–1,700 lbs) and road incline (0–10% grade). Triangular membership functions define light/medium/heavy cargo, flat/moderate/steep roads, and low/medium/high MPG, and nine if-then rules cover every input combination. Three test cases predict 21.9 MPG (empty, flat highway), 17.0 MPG (half load, rolling hill), and 12.1 MPG (near-full load, steep pass). A comparison with a crisp (binary) version of the same rules shows the fuzzy output changes gradually where crisp logic jumps by about 5 MPG at its cutoffs.

- [`fuzzy_logic.ipynb`](./fuzzy_logic.ipynb) — the full notebook: fuzzy logic background and problem statement, fuzzy sets, membership function diagrams and rules, the scikit-fuzzy implementation with three test cases, output plots, and a comparison with traditional logic.
- `fuzzy_logic_assignment.docx` — original assignment instructions (not tracked in git).
- `script.md` — narration script for the video presentation (not tracked in git).
