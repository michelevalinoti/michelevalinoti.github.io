---
title: "The Market for Political Access. Evidence from New York State Lobbying"
subtitle: ""
date: "2023-06-18"
categories:
  - research
tags:
  - Lobbying
  - Structural Models
summary: >
  Political access is scarce. This project studies how commercial lobbying firms
  broker that access between clients and New York State lawmakers, and how
  intermediaries’ relationship capital shapes who gets meetings and who
  ultimately benefits from public resources.

image:
  filename: "featured.png"
  caption: ""
  focal_point: "Center"

project:
  status: "Work in progress"
  period: "2023–present"
  collaborators:
    - "Michele Valinoti"

links:
  - icon: file-text
    name: Working paper
    url: "/publication/lobbying-paper/"
  - icon: file-powerpoint
    name: Slides
    url: "/publication/lobbying-paper/slides_chapter1_website.pdf"
---


## Overview

This project studies how political access is allocated when lawmakers’ time and attention are scarce, and how **commercial lobbying firms** mediate access between clients and legislators. Using unusually granular disclosure data, I track *who contacts whom, through which intermediary, and on behalf of which client*, and connect access patterns to downstream public-resource outcomes for a large set of organizations.

A central lens is to treat lobbying as an **intermediated access market**: clients choose whether (and how) to lobby, while intermediaries help route attention toward particular lawmakers under capacity constraints.

{{< figure
  src="network_lobbyist_client_combo_.png"
  caption="Example of a tripartite network built from New York State lobbying disclosures: clients retain lobbyists/firms who contact legislators."
>}}

## Data & Setting

The setting is New York State, where disclosures make it possible to observe lobbying at the level of **contacts to specific targets**, rather than only spending aggregates. The project focuses on legislative contacts and connects them to administrative records on grants and contracts for tax-exempt organizations.

## Methods

The analysis combines:

- **Descriptive evidence** on how contacts are distributed across lawmakers and how the mix of in-house vs. commercial intermediation varies with lawmakers’ institutional positions.
- A **two-stage structural model** aligned with the institutional environment: in Stage 1, clients choose an organizational form (e.g., in-house, commercial firm, or both) and negotiate fees; in Stage 2, lawmakers allocate meetings across client–lobbyist pairs subject to capacity constraints. Access then enters a concave production function, allowing additional meetings to have diminishing marginal impact on downstream outcomes.

## Results & Takeaways

- **Access is unevenly distributed**: contacts disproportionately flow to lawmakers with greater institutional leverage, and commercial lobbying firms appear especially active in reaching this high-demand segment.
- **Observable relationship capital lines up with access patterns**: campaign-based ties and revolving-door connections are associated with higher contact probabilities and greater contact intensity, even after accounting for persistent differences across clients, intermediaries, and lawmakers.
- **Access and outcomes move together**: lobbying engagement and intensity are positively associated with grants among tax-exempt organizations.
- **Counterfactuals emphasize distributional shifts**: model-based simulations indicate that removing commercial intermediaries materially changes who participates and which lawmakers are targeted, with comparatively modest changes in aggregate outcomes but more noticeable redistribution across organization size and baseline access.

{{< figure
  src="contacts_pct_change_by_asset_bin_1219.png"
  caption="Model-based counterfactual simulations under alternative lobbying environments (e.g., removing commercial intermediaries and reallocating relationship capital). The figure summarizes how predicted contact activity shifts across organization size bins."
>}}
