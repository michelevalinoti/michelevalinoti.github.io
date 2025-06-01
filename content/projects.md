---
title: 'Projects'
date: 2024-05-19
type: landing

design:
  # Section spacing
  spacing: '5rem'

# Page sections
sections:
  - block: collection
    id: phd-projects
    content:
      title: Research projects
      subtitle: 
      #text: I enjoy making things. Here are a selection of projects that I have worked on over the years.
      filters:
        folders:
          - project

      filter_button:
        - name: All
          tag: "*"
        - name: DeepLearning
          tag: "Deep Learning"
        - name: Other
          tag: "Demo"
      filter_default: 0

    design:
      view: article-grid
      fill_image: false
      columns: 3
  - block: collection
    id: dormant-projects
    content:
      title: Dormant projects
      subtitle: 
      #text: I enjoy making things. Here are a selection of projects that I have worked on over the years.
      filters:
        folders:
          - project

      filter_button:
        - name: All
          tag: "*"
        - name: DeepLearning
          tag: "Deep Learning"
        - name: Other
          tag: "Demo"
      filter_default: 0
      
    design:
      view: article-grid
      fill_image: false
      columns: 3
  - block: collection
    id: phd-projects
    content:
      title: Research projects
      subtitle: 
      #text: I enjoy making things. Here are a selection of projects that I have worked on over the years.
      filters:
        folders:
          - project

      filter_button:
        - name: All
          tag: "*"
        - name: DeepLearning
          tag: "Deep Learning"
        - name: Other
          tag: "Demo"
      filter_default: 0
      
    design:
      view: article-grid
      fill_image: false
      columns: 3
---