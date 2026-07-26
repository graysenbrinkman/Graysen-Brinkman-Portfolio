---
title: "Gauss Method Preliminary Orbit Determination"
date_range: "Mar 2026 – Apr 2026"
category: "Projects"
section: "projects"
featured: false
skills: ["MATLAB", "LaTeX", "Astrodynamics", "Numerical Methods"]
image: "/assets/images/gauss-diagram.png"
description: "Implemented the Gauss method in MATLAB to determine orbital elements from angle-only tracking observations, with iterative refinement and sensitivity analysis."
objective: "The goal of this project was to implement the classical Gauss method for preliminary orbit determination (POD) using angle-only measurements. Given only topocentric right ascension and declination observations at three time steps, the program estimates the full state vector of an orbiting object and derives its classical orbital elements. The project also compared two velocity estimation approaches, validated results against a reference solution, and analyzed the sensitivity of the method to small measurement errors."
methods: "The implementation was written in MATLAB and structured around three core components: an initial state vector estimate using the Gauss method formulation, velocity determination using both the Lagrange series and Gibbs method, and an iterative refinement loop that updates the solution until the change in slant range falls below a tolerance of 1e-4 km. Orbital elements were extracted from the converged state vector and validated against Example 5.11 from Curtis' Orbital Mechanics for Engineering Students. A sensitivity analysis was also performed by independently perturbing the right ascension and declination at the second observation to observe the effect on the computed orbital elements. Results and analysis were documented in a formal technical report written in LaTeX."
takeaways: "This project reinforced how sensitive angle-only orbit determination is to small measurement errors. Even a fraction of a degree change in right ascension or declination produced large, nonlinear shifts in the computed orbital elements, and in many cases caused the iterative method to fail to converge entirely. It also highlighted how orbital parameters like the semi-major axis are disproportionately affected by small velocity errors due to their dependence on orbital energy. On the implementation side, I gained experience structuring a multi-function MATLAB program and writing a formal technical report in LaTeX."
gallery:
  - image: "/assets/images/gauss-convergence-plot.jpg"
    caption: "Convergence of slant range error over 33 iterations of the iterative Gauss method"
  - image: "/assets/images/gauss-table.png"
    caption: "Comparison of non-iterative and converged state vector results"
---