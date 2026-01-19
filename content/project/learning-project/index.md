---
title: The Effects of Learning in Dynamic Data Markets
subtitle: MS Thesis
date: 2019-03-19
external_link: ''
tags:
  - Dynamic Programming
  - Java
  - Revenue Management
  - Bayesian Learning
categories:
  - pre-phd
links:
  - icon: brands/github
    name: Code
    url: "https://github.com/michelevalinoti/Learning-Dynamic-Data-Markets"
summary: >
  Studies a dynamic data-market platform that uses posted payments to attract data providers and posted prices to serve queries, while learning key market primitives over time. The thesis characterizes how Bayesian learning changes optimal payment dynamics, and when learning policies can conflict with incentive-compatibility for strategic sellers.
image:
  filename: "featured.png"
  caption: ""
  focal_point: "Center"
---

## Overview

This thesis studies an online **data market** in which a platform incentivizes data providers to structure and sell databases, while buyers pay to answer queries that benefit from joining the databases available on the platform. The platform faces an explicitly dynamic environment: sellers arrive over time, transactions are only partially observed, and the platform may need to **learn** market conditions while still setting payments and prices that keep the system functioning.

The core goal is to design a posted-payment policy for sellers that **maximizes buyers’ expected discounted surplus**, while retaining basic market-design constraints (individual rationality, budget discipline, and incentive-compatibility considerations) in a learning environment.

## Data & Setting

The analysis is model-based. The platform’s state evolves with the **number of databases already acquired** and (in the learning extension) the platform’s **belief about seller arrivals**, updated from observed transaction outcomes. Performance comparisons are illustrated through simulations under common benchmark choices for sellers’ cost distributions and buyers’ value functions.

## Methods

The framework extends a dynamic posted-price model of data acquisition by adding **Bayesian learning** about seller arrivals. The platform’s decision problem is formulated as a dynamic program in which the state includes both (i) current market size and (ii) a belief over a small set of plausible arrival-rate regimes. This turns the platform’s optimization into a Markov decision process over an expanded state space.

{{< figure src="nu_20.png" caption=""Value function as a function of the number of acquired databases for a fixed level of belief." }}

Two sets of policies are derived:

- **Payments to sellers:** computed from Bellman equations that trade off faster market growth (attractive early payments) against expected future value, while accounting for how today’s payment affects what the platform can infer from observed sales.
- **Prices to buyers:** constructed to extend a martingale-style pricing logic that aims to reduce incentives for strategic timing by buyers, while keeping the platform’s expected budget imbalance controlled in the long run.

## Results & Takeaways

Learning changes the platform’s behavior in predictable but nontrivial ways. Relative to full-information benchmarks, the learning platform generally has reasons to adjust payments not only for immediate acquisition value, but also for how payments affect informativeness of what is observed.

{{< figure src="ic_20,30.png" caption="Comparison of seller payments and MDP values under a learning policy versus a full-information benchmark at a fixed market size." }}

A key caution is that **learning and incentive compatibility can collide** when sellers are strategic about *when* to participate. In particular, a Markov learning policy can create situations where delaying participation makes the platform more pessimistic, and pessimism can raise the payment a seller expects to receive later. The thesis proposes an **incentive-compatible variant** (via an “ironed” payment adjustment) that preserves truthful timing incentives at the cost of some surplus relative to the fully optimal learning rule.

{{< figure src="buyersurplus_environments_075_09.png" caption="Simulation comparison of buyers’ surplus over time across full-information, learning, and non-learning scenarios under alternative arrival-rate and discount-factor settings." }}

Extensions discuss how results change when (i) seller arrivals are observable, (ii) buyers arrive stochastically, and (iii) the buyer value function is known only up to parameters—highlighting a broader “learning vs. earning” tension on the demand side as well.
