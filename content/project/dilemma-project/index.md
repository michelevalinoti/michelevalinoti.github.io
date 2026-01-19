---
title: Cooperation in Evolutionary Game Theory
subtitle: BS Thesis
date: 2017-07-29
tags:
  - Game Theory
  - Java
categories:
  - pre-phd
summary: >
  A thesis on why cooperation can arise (and fail) under natural selection when interactions are repeated.
  Using evolutionary game theory and simulations of the Iterated Prisoner’s Dilemma, it documents when
  strategies like Tit For Tat can sustain cooperation, how mistakes undermine it, and why “forgiving”
  variants can matter once cooperation is established.
image:
  filename: "featured.png"
  caption: ""
  focal_point: "Center"

project:
  status: "Completed"
  period: "2016–2017"

---

## Overview

This project studies the evolution of cooperation through the lens of **evolutionary game theory**, focusing on **direct reciprocity** in the Iterated Prisoner’s Dilemma. The central question is not whether cooperation is “optimal” in a one-shot sense, but when cooperative behavior can be **stable**, **robust**, and **able to get started** in populations where defection is common.

## Methods

The evidence is simulation-based. Populations are composed of “species” (strategy types) that repeatedly interact in random encounters across generations. Strategy performance is summarized by accumulated payoff, interpreted as a proxy for relative fitness that governs reproduction into the next generation.

The core tool is a simple evolutionary updating rule: strategies play repeated games, earn payoffs, and the population composition updates proportionally to relative performance under assumptions like asexual reproduction, constant population size, and no mutation.

The thesis uses a small set of canonical strategies—e.g., unconditional cooperation/defection (ALLC/ALLD), **Tit For Tat (TFT)**, and more forgiving/reactive variants—to illustrate how stability and robustness depend on the interaction environment (e.g., expected length of repeated interaction) and on whether agents sometimes make mistakes.

## Results & Takeaways

A few patterns show up consistently across the simulation exercises:

- **Unconditional cooperation is fragile.** In mixed populations, strategies that always defect can exploit unconditional cooperators, and selection tends to amplify that advantage.
- **TFT can stabilize cooperation under repeated interaction, but it is sensitive to noise.** When mistakes occur (accidental defections/cooperations), TFT can get trapped in retaliatory cycles that lower average payoffs, eroding its advantage.
- **Forgiveness can help once cooperation exists.** “Generous” variants can dampen error-driven spirals and restore mutual cooperation, although they can be less protected in environments with many defectors.

{{< figure src="fitness.png" caption="Simulation comparison showing how introducing mistake probabilities changes relative performance and long-run frequencies of TFT and a more forgiving variant (GTFT) alongside unconditional types." }}

Finally, the thesis highlights that **starting cooperation** can be harder than sustaining it: even if cooperative strategies can do well once they are common, they may fail to invade from rarity in a well-mixed population. This motivates the role of clustered encounters or other deviations from random mixing as a practical route for cooperation to gain a foothold.

{{< figure src="cooperative_clusters_invasion.png" caption="Illustration of an ‘initial viability’ problem: when cooperators are rare in a largely defective population, they may fail to invade under random matching—suggesting a role for clustered interactions in jump-starting cooperation." }}```

