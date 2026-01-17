---
title: 'Research & Teaching'
date: 2024-10-24
type: landing

design:
  # Section spacing
  spacing: '5rem'

sections:
  - block: collection
    id: research
    content:
      title: Research
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: community/citation_modified
  - block: collection
    id: teaching
    content:
      title: Teaching
      text: ""
      filters:
        folders:
          - teaching
    design:
      view: article-grid
      columns: 2
---
