---
title: Spatial Frictions and Product Differentiation
date: 2022-11-16
external_link: ''
tags:
  - Product Differentiation
  - Spatial Frictions
  - Web Scraping
categories:
  - dormant
image:
  filename: "featured.png"
  caption: ""
  focal_point: "Center"

project:
  status: "Dormant"
  period: "2022-2023"
  collaborators:
    - "Michele Valinoti"

links:
  - icon: brands/github
    name: Code
    url: "https://github.com/michelevalinoti/Spatial-Competition-Restaurants"
summary: >
  Combines restaurant listings, delivery-network availability, and mobility data to characterize how exposure to delivery competition relates to local cuisine variety across NYC.
---

## Overview

This project studies how **spatial frictions** interact with **product differentiation** in a setting where geography remains central but consumer reach expands through delivery. The core idea is that when access to non-local restaurants becomes easier, competitive pressure may shift away from purely local proximity and toward **differentiation in product space** (e.g., cuisines and menu positioning).

The analysis focuses on New York City restaurants. Delivery availability is used as a practical proxy for reduced spatial frictions that can increase competitive overlap without changing physical locations.

## Data & Setting

The unit of analysis is the **census tract**. Restaurant supply is built from Yelp listings (location and attributes), complemented with a large crawl of a major delivery platform to recover where restaurants deliver and the associated terms (e.g., delivery times/fees). Demand-side behavior is summarized using mobile-location visit data (POI visits over time), which helps characterize how far consumers travel for restaurant consumption in different parts of the city.

{{< figure
src="foot_traffic_all_daytime.png"
caption="Figure 3a: Foot-traffic patterns from mobile-location data. The figure summarizes how far visits travel and how visit geography varies across NYC, providing a descriptive benchmark for the role of distance in restaurant demand."
>}}

A key object is **local product diversity**: how varied restaurants are within a tract, based on similarity of cuisine labels and how concentrated (or dispersed) cuisine groups are within neighborhoods.

{{< figure
src="log_disparity_0.png"
caption="Figure 1a: Tract-level product diversity in NYC. The map visualizes neighborhood variation using a composite index built from complementary measures of within-tract similarity and cuisine concentration."
>}}

## Methods

- **Conceptual framework:** A stylized two-dimensional competition environment (geography × product space) motivates why lower spatial frictions can make differentiation more valuable when consumers can substitute toward a broader set of options.
- **Measuring differentiation:** Cuisine-label vectors are used to compute similarity between restaurants; tract-level diversity aggregates these similarities and uses clustering-based groupings to capture concentration versus variety.
- **Associational analysis:** Tract-level diversity is related to measures of **delivery exposure**, including the presence of options that originate beyond the immediate neighborhood, while controlling for observable tract characteristics.

## Results & Takeaways

Across specifications, higher exposure to delivery-based competition—especially from comparatively non-local options—**is associated with higher measured product diversity**. The pattern is consistent with the idea that an expanded choice set can be accompanied by more differentiation in what is offered locally.

The evidence here is best read as characterization rather than causal attribution: delivery coverage and local variety likely co-move with unobserved demand, neighborhood change, and platform-side decisions.

{{< figure
src="OLS_params_diversity_num_set_difference_delivery_physical__BoroName.png"
caption="Figure 9a: Associations between tract-level product diversity and delivery exposure as the definition of ‘non-local’ competition varies across distance thresholds (OLS with tract controls)."
>}}
