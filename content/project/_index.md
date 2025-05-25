---
title: "Projects"
type: landing
widget: portfolio
# headless: false is implicit

menu:
  main:
    identifier: "project"
    name: "Projects"
    weight: 20

content:
  filters:
    folders:
      - project
    kinds:
      - page
      - section

  filter_button:
    - name: All
      tag: "*"
    - name: DeepLearning
      tag: "Deep Learning"
    - name: Other
      tag: "Demo"
  filter_default: 0

design:
  view:    card-grid   # supported views: card-grid, list, masonry, etc.
  columns: "2"
---
