---
title: "Work in progress"
widget: publication        # ✅ tells Hugo “use the publication widget”
type: landing              # optional; picks your landing‐page layout
menu:
  main:
    identifier: publications
    name: Publications
    weight: 25

# Which folders under content/publication/ to include
content:
  filters:
    folders:
      - journal-article
      - conference-paper
      - preprint
      - lobbying-paper
    kinds:
      - page

design:
  view: card-grid          # or list, masonry, table
  columns: "2"
---