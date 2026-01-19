---
title: "Tying the Knot: Marriage Patterns in Italy, 19th–20th Century"
date: 2024-09-10
external_link: ''
tags:
  - Economic History
  - LLMs
  - OCR
categories:
  - dormant
links:
  - icon: brands/github
    name: Code
    url: "https://github.com/enzodipasquale/Antenati"
summary: >
  This project builds a new dataset of Italian marriages from digitized civil records and develops a
  reproducible pipeline to preprocess images, transcribe handwritten text at scale, and harmonize
  key attributes (names, ages, occupations, domiciles). The goal is to characterize how marriage
  patterns vary across time and local contexts, while documenting the measurement choices needed
  to interpret historical administrative sources.
image:
  filename: "featured.png"
  caption: ""
  focal_point: "Center"
---

with Enzo Di Pasquale

## Overview

This project uses digitized Italian civil marriage records to study long-run patterns in who marries whom and under what local conditions. A practical focus is that the raw source material is messy: scans can contain multiple pages, variable layouts, and handwriting quality that changes across places and decades. The work therefore treats **data construction** as a first-order object, aiming for a pipeline that is scalable, auditable, and explicit about uncertainty.

## Data & Setting

The primary source is the Antenati ecosystem of digitized civil records. The unit of observation is the marriage act, with extracted fields intended to cover spouses and parents (e.g., names, ages, occupations, and domiciles), alongside archival metadata that anchors records in place and time.

## Methods

The pipeline has two stages:

1) **Preprocessing (image-level):** detect and split double-page scans, locate text-dense regions, crop irrelevant margins, and standardize page outputs to stabilize downstream transcription.

2) **Transcription (page-level):** process pages in batches with prompts that incorporate record metadata and emphasize faithful extraction (including explicit markers for illegible or uncertain text), then map transcriptions into structured variables.

{{< figure
  src="age_density.png"
  caption=""
>}}

{{< figure
  src="age_correlations_high_res.png"
  caption=""
>}}
