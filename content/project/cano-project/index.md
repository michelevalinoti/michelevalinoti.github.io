---
title: "Criminal Activity Nuisance Ordinance (CANO) Database"
date: "2024-08-09"
categories:
  - research
tags:
  - Local Governance
  - Large Language Models
summary: >
  Built a national database of Criminal Activity Nuisance Ordinances (CANOs) by collecting municipal codes, identifying relevant provisions at scale, and extracting structured policy attributes. The project uses the resulting legal design measures to describe patterns of adoption and to characterize how adoption timing relates to housing and public-safety outcomes.

image:
  filename: "featured.png"
  caption: ""
  focal_point: "Center"

project:
  status: "Work in progress"
  period: "2024–present"
  collaborators:
    - "Michele Valinoti"
    - "Bryant Moy"
    - "Moin Khan"

links:
  - icon: file-text
    name: Working paper
    url: "/publication/cano-paper/"
  - icon: file-powerpoint
    name: Slides
    url: "/publication/cano-paper/slides_chapter2_website.pdf"
---

with Bryant Moy, Moin Khan

## Overview

Criminal Activity Nuisance Ordinances (CANOs) are local laws that treat repeated “nuisance” incidents as a **property-level** problem, often shifting compliance and enforcement pressure toward property owners and tenants. This project builds a national database of CANOs from municipal codes, enabling systematic description of where these ordinances appear, how they are written, and how adoption correlates with local conditions and downstream housing-related measures.

{{< figure
src="map_us_cano_all_in_one.png"
caption="Geographic distribution of jurisdictions identified as having at least one CANO in the municipal-code corpus, illustrating broad prevalence and clustering across states."
>}}

## Data & Pipeline

The database is constructed in three steps:

1. **Collection**: scrape and standardize municipal codes from major codification platforms and municipal websites, and select candidate provisions using nuisance-related keywords.
2. **Classification**: identify CANO articles using a long-document classification pipeline (a conservative long-context model benchmarked against hand-labeled datasets), designed to distinguish CANOs from adjacent ordinance types.
3. **Attribute extraction**: extract structured policy features from ordinance text using an LLM-based schema (e.g., incident thresholds, liable party, penalty tools, and whether eviction is mandated/encouraged/optional/silent).

## Methods

Empirically, the project uses the resulting jurisdiction-by-year adoption panel to:

- **Describe adoption patterns** and how adoption rates vary with local demographics and baseline conditions.
- **Characterize associations with outcomes** by linking adoption timing to administrative eviction panels and crime/arrest panels, using standard staggered-adoption event-time and difference-in-differences-style designs as descriptive summaries (interpreted cautiously given potential confounding and measurement error in both policy timing and coverage).

## Results & Takeaways

- **Widespread but uneven adoption**: CANOs appear in a large number of jurisdictions in the corpus, with substantial cross-state variation.
- **Outcome patterns concentrate in housing measures**: around adoption, event-time patterns are more consistently visible in eviction-related outcomes than in arrest/crime measures. The magnitudes and precision vary by specification and by ordinance design, so these results are best read as descriptive patterns rather than definitive causal effects.

{{< figure
src="es_three_outcomes.png"
caption="Event-time estimates around CANO adoption for eviction-related outcomes, shown relative to a pre-adoption baseline; post-adoption patterns are summarized alongside pre-trend diagnostics."
>}}
