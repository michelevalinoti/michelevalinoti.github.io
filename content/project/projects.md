---
title: "Projects"
type: landing        # adjust if your theme expects a different layout
widget: portfolio
# headless: false   # you can omit headless entirely since false is default

content:
  filters:
    folders: [ project ]
    kinds:   [ page ]
  filter_button:
    - name: All           ; tag: "*"
    - name: Deep Learning ; tag: "Deep Learning"
    - name: Other         ; tag: Demo
  filter_default: 0

design:
  columns:     "1"
  view:        masonry
  flip_alt_rows: false

# Add this so Hugo builds a menu link for you:
menu:
  main:
    identifier: "projects"
    name: "Projects"
    weight: 20
---