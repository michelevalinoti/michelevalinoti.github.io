---
title: "Projects"
type: landing
widget: portfolio
# headless: false is implicit

# Your landing page sections - add as many different content blocks as you like
sections:
  # A section to display blog posts
  - block: collection
    id: phd-projects
    content:
      title: Research projects
      subtitle: 
      # Display content from the `content/post/` folder
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
      columns: '2'
      # Choose your content listing view - here we use the `showcase` view
      view: card
      # For the Showcase view, do you want to flip alternate rows?
      flip_alt_rows: true
      
  - block: collection
    id: dormant-projects
    content:
      title: Dormant projects
      subtitle: 
      # Display content from the `content/post/` folder
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
      columns: '2'
      # Choose your content listing view - here we use the `showcase` view
      view: card
      # For the Showcase view, do you want to flip alternate rows?
      flip_alt_rows: true

  - block: collection
    id: pre-phd
    content:
      title: Pre-PhD
      subtitle: 
      # Display content from the `content/post/` folder
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
      columns: '2'
      # Choose your content listing view - here we use the `showcase` view
      view: card
      # For the Showcase view, do you want to flip alternate rows?
      flip_alt_rows: true
      
---
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