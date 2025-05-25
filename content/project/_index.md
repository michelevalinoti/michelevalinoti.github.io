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
    #kinds:
    #  - page

  filter_button:
    - name: "All"
      tag: "*"
    - name: "Deep Learning"
      tag: "Deep Learning"
    - name: "Other"
      tag: "Demo"
  filter_default: 0

design:
  columns: "1"
  view: masonry
  flip_alt_rows: false
---
