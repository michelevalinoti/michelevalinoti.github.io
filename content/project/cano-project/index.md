---
title: "Criminal Activity Nuisance Ordinance (CANO) Database"
date: "2024-08-09"
categories:
  - research
tags:
  - Local Governance
  - Large Language Models
summary: >
  Built a national database of Criminal Activity Nuisance Ordinances (CANOs) by collecting municipal codes, identifying relevant provisions at scale, and extracting structured policy attributes. The project links legal design to patterns in adoption and housing-related outcomes.

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

Criminal Activity Nuisance Ordinances (CANOs) are municipal laws that treat repeated “nuisance” incidents as a **property-level problem**, potentially shifting enforcement pressure onto property owners and residents. This project builds a national database of CANOs from municipal codes, enabling systematic evidence on where these ordinances exist, how they are written, and how they relate to adoption patterns and housing outcomes.

{{< figure
  src="map_us_cano_all_in_one.png"
  caption="Geographic distribution of jurisdictions identified as having a CANO, illustrating broad prevalence and regional clustering."
>}}

## Data & Pipeline

The database is built in three steps:

1. **Collection**: scrape and standardize municipal codes across multiple legal publishers.
2. **Classification**: identify CANO provisions using a Long-Document Encoder (LED), a transformer architecture.
3. **Attribute extraction**: recover structured policy features (e.g., enforcement structure, owner obligations, eviction-related language, timing) from ordinance text using an LLM-based schema.

## Results & Takeaways

The database supports three high-level takeaways:

- **Widespread but uneven adoption**: CANOs are present in many jurisdictions, with substantial regional clustering and local variation in legal design.
- **Housing-facing outcome associations**: in event-time analyses around adoption, changes are more consistently visible in **housing instability measures** (e.g., eviction-related outcomes) than in **public-safety measures** (e.g., arrests), consistent with these policies operating primarily through housing and landlord-tenant channels rather than through direct deterrence of crime.

{{< figure
  src="es_three_outcomes.png"
  caption="Event-time estimates around CANO adoption for eviction-related outcomes relative to the pre-adoption baseline."
>}}
