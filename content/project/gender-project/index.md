---
title: Women, Media and Politics (with S. Parsa)
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
    name: Draft
    url: "/publication/women-media-politics/"
---

with Sahar Parsa

## Overview

This project links U.S. elections to newspaper coverage to measure systematic differences in how male and female political candidates are discussed. The objective is measurement: to build transparent, scalable metrics of language that can be compared across offices, electoral environments, and time.

A key design choice is interpretability. The analysis uses a **disentangled text representation** that separates variation in *topic/content* from *framing/style*, then quantifies gendered differences along each dimension.

## Data & Setting

The dataset combines election records with a large corpus (1M+) of election-related news coverage, matched to candidates through a candidate-resolved text pipeline. The empirical focus is on patterns that persist across comparable political contexts.

## Methods

The measurement strategy has three pieces:

1. **Embedding-based representations.** Candidate-linked text is mapped into a semantic vector space. Differences are summarized using standard geometric comparisons (e.g., distances, centroid similarity), which are easy to compute consistently across contexts.

{{< figure
  src="tsne_base.png"
  caption="Two-dimensional t-SNE visualization of candidate-linked text embeddings."
>}}

2. **Dynamics and conditioning.** The same separation metrics are tracked over time and across offices, and can be computed within more comparable electoral contexts to distinguish composition effects from within-context differences.

3. **Disentangling content and framing.** To separate “what” from “how,” the project estimates a representation that decomposes each text into topic and style components, and then studies whether gender differences load more strongly on one channel or the other.

{{< figure
  src="variance_explained_differences.png"
  caption="Variance explained by topic vs. style components. The figure reports the share of variation captured by principal components in the disentangled representation."
>}}
