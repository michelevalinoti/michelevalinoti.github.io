---
title: Women, Media and Politics
date: 2024-10-11
external_link: ''
categories:
  - research
tags:
  - Text-as-Data
  - Gender Bias
links:
  - icon: file-text
    name: Working paper
    url: "/publication/gender-paper/"
summary: >
  This project measures how political candidates are described in the news using a large corpus of election-related coverage. It treats embedding geometry as an outcome, tracks differences across contexts and over time, and uses a disentangled representation to separate topic/content from framing/style.
image:
  filename: "featured.png"
  caption: ""
  focal_point: "Center"

project:
  status: "Work in progress"
  period: "2024–present"
  collaborators:
    - "Michele Valinoti"
    - "Sahar Parsa"

links:
  - icon: file-text
    name: Working paper
    url: "/publication/women-media-politics/"
---

with Sahar Parsa

## Overview

This project links U.S. elections to newspaper coverage to characterize differences in how male and female political candidates are discussed. The goal is measurement: to build transparent, scalable metrics of candidate-linked language that can be compared across offices, electoral environments, and time.

A key design choice is interpretability. The analysis uses a **disentangled text representation** that separates variation in *topic/content* (what is being discussed) from *framing/style* (how it is being discussed), then summarizes gender-associated differences along each dimension.

## Data & Setting

The dataset combines election records with a large corpus of election-related news coverage, matched to candidates through a candidate-resolved text pipeline. The empirical focus is on patterns that can be computed *within comparable political contexts* (e.g., office, party environment, incumbency status), to reduce purely compositional comparisons.

## Methods

1. **Embedding-based representations.** Candidate-linked text is mapped into a semantic vector space. Differences are summarized using geometric comparisons (e.g., centroid distances/similarities), which can be computed consistently across contexts.

{{< figure
src="tsne_base.png"
caption="Two-dimensional t-SNE visualization of candidate-linked text embeddings. The projection is used for visualization and does not preserve all high-dimensional distances."
>}}

2. **Dynamics and conditioning.** The same embedding-based separation measures are tracked over time and across offices, and are also computed within more comparable subsets to distinguish broad composition shifts from within-context differences.

3. **Disentangling content and framing.** To separate “what” from “how,” the project estimates a representation that decomposes text into topic and style components. The analysis then assesses whether gender-associated differences load more strongly on content-related dimensions, style-related dimensions, or both.

{{< figure
src="variance_explained_differences.png"
caption="Variance explained by topic vs. style components in the disentangled representation, summarizing how much structure each channel captures in candidate-linked language."
>}}
