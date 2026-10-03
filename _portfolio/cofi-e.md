---
title: "CoFi-E: Repairing Blind Spots in Conformal Detectors"
excerpt: "Collision-guided refinement of a detector's score so that anytime-valid conformal monitoring can see distribution changes its original score hides."
collection: portfolio
permalink: /portfolio/cofi-e/
link: /projects-html/cofi-e/
date: 2026-09-20
tags:
  - Conformal Prediction
  - Anomaly Detection
  - Distribution Shift
---

- Identifies rank-fiber collisions: distribution changes that leave a detector's score distribution unchanged, so every conformal bettor on that score is blind while false-alarm control still holds.
- Refines the score by splitting groups of observations that share a score whenever training alternatives reveal a difference inside them; independent audit data certify each accepted split.
- Refinements never discard rank information the detector already exposes, and hidden information shrinks geometrically when informative splits are available.
- Runtime false-alarm control is kept separate from learning: the refined score is frozen before fresh reference data are drawn.
- Evaluated on MVTec AD, UCR, and UEA benchmarks, with transfer bounds that quantify how detection evidence depends on an unseen anomaly family's distance from the training alternatives.

[Read the full project write-up](/projects-html/cofi-e/)
