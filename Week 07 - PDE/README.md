# Modeling Pollution Spread in a River with the Diffusion Equation

AIT 525 assignment — solving the one-dimensional diffusion equation numerically (finite differences) and with a Fourier transform, applied to a pollutant spill spreading along a river.

Models a chemical spill (a 100 mg/L peak) in the middle of a 10 km river with the diffusion equation, using D = 0.1 km²/hour and clean (zero) river ends. The explicit finite difference method (r = 0.4) shows the peak dropping to about 41 mg/L in the first hour and the river converging to a clean steady state, with the peak below 1 mg/L after about 233 hours; a test with r = 0.6 shows the method blowing up. A Fourier transform solution of a simplified, very long river matches the exact answer almost perfectly and reaches any time in one step, and a comparison discusses when Fourier, Laplace, and numerical methods each fit best.

- [`pde_diffusion.ipynb`](./pde_diffusion.ipynb) — the full notebook: PDEs in AI and the diffusion equation, the explicit finite difference solution with plots, and the Fourier transform solution with a comparison of both methods.
- `PDE_Assignment.docx` — original assignment instructions (not tracked in git).
- `script.md` — narration script for the video presentation (not tracked in git).
