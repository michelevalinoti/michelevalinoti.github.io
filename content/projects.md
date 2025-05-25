---
title: "Projects"
type: landing
widget: portfolio
# headless: false is implicit

content:
  filters:
    folders:
      - project
    kinds:
      - page

  filter_button:
    - name: All
      tag: "*"
    - name: DeepLearning
      tag: "Deep Learning"
    - name: Other
      tag: "Demo"
  filter_default: 0

design:
  # Choose how many columns the section has. Valid values: '1' or '2'.
  columns: '1'
  # Choose a listing view
  view: masonry
  # For Showcase view, flip alternate rows?
  flip_alt_rows: false
---