---
title: "Intermediation in Matching Markets"
subtitle: "Evidence from Commercial Lobbying in New York State"
date: "2023-06-18"
categories:
  - research
tags:
  - Matching Models
  - Lobbying
  - Political Economy
summary: >
  How commercial lobbyists shape the allocation of political access between clients
  and lawmakers using network position and targeted intermediation.

image:
  filename: "featured.png"
  caption: "Illustration of lobbying relationships between clients, lobbyists, and lawmakers."
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
  - icon: brands/github
    name: Code
    url: "https://github.com/michelevalinoti/Matching-Lobbying"
---

## Overview

This project studies how commercial lobbying firms intermediate access between private clients and legislators in New York State.  
Using detailed data on lobbying contacts, campaign contributions, and legislative careers, I document how access is distributed and how intermediaries shape which politicians receive attention.

![Overview of lobbying network between clients, lobbyists, and lawmakers.](network-overview.png)

The core idea is to treat lobbyists as intermediaries in a matching market: clients choose which firms to hire, and firms decide which lawmakers to approach given their connections and capacity.

## Data & Setting

The dataset combines:

- Administrative records of lobbying contacts between clients, lobbying firms, and legislators.
- Legislators’ committee assignments, seniority, and leadership positions.
- Public data on campaign contributions and previous employment links.

This allows me to construct a tripartite network (clients–lobbyists–lawmakers) and track how attention is allocated over time.

## Methods

Methodologically, the project:

- Uses a reduced-form analysis to characterize which lawmakers receive more attention (e.g., by committee, seniority, and leadership roles).
- Builds a structural matching model where:
  - clients choose lobbying firms,
  - firms decide how to allocate contacts across lawmakers,
  - contacts are priced through fees that depend on firm characteristics and expected returns.

The model embeds equilibrium conditions that link observed contacts and fees to the underlying distribution of lobbying demand and intermediation capacity.

## Results & Takeaways

Preliminary findings:

- Commercial lobbyists account for a large share of observed contacts, especially when they are personally connected to lawmakers.
- Connections via campaign contributions or prior employment are used selectively, even after controlling for issue-area and client characteristics.
- Reallocating intermediation power across firms has sizable implications for which lawmakers receive political attention.

![Estimated effect of intermediary connections on probability of contact.](effect-plot.png)

From a policy perspective, the results speak to how regulation of lobbying firms and their connections can change who gets access to policymakers, even holding total lobbying effort fixed.

## Outputs

- Working paper: *Intermediation in Matching Markets: Evidence from Commercial Lobbying*.
- Slides: chapter 1 slides for seminars and job talks.
- Code: data processing and estimation in Python/R, with reproducible analysis scripts.
