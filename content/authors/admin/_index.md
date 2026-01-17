---
# Display name
title: Michele Valinoti

# Name pronunciation (optional)
name_pronunciation: Mee-kai-lai

# Full name (for SEO)
first_name: Michele
last_name: Valinoti

# Status emoji
#status:
#  icon: ☕️

# Is this the primary user of the site?
superuser: true

# Highlight the author in author lists? (true/false)
highlight_name: true

# Role/position/tagline
role: PhD Candidate at NYU

# Organizations/Affiliations to display in Biography blox
#organizations:
#  - name: OpenAI
#    url: https://openai.com/

# Social network links
# Need to use another icon? Simply download the SVG icon to your `assets/media/icons/` folder.
profiles:
  - icon: at-symbol
    url: 'mailto:michele.valinoti@nyu.edu'
    label: E-mail me
  #- icon: brands/x
  #  url: https://twitter.com/GetResearchDev
  #- icon: brands/instagram
  #  url: https://www.instagram.com/
  - icon: brands/linkedin
    url: https://www.linkedin.com/in/michele-valinoti-b8a515196/
  - icon: brands/github
    url: https://github.com/michelevalinoti
  #- icon: academicons/google-scholar
  #  url: https://scholar.google.com/
  #- icon: academicons/orcid
  #  url: https://orcid.org/

interests: []

education:
  - area: PhD Economics
    institution: New York University
    date_start: 2020-09-01
    date_end: 2026-01-01
    summary: |
      Worked on 5 research projects spanning causal inference, structural estimation, NLP and LLMs.

      Research Assistant for Giulia Brancaccio/Karam Kang (Economics) and Bryant Moy (Politics).

      Teaching Assistant of Maths (MA) and Statistics (UG). Course assistant of Industrial Organization (UG), Game Theory (PhD), and Money & Banking (UG).
    #button:
      #text: 'Read Thesis'
      #url: 'https://example.com'
  - area: MA Economics
    institution: Collegio Carlo Alberto
    date_start: 2015-09-01
    date_end: 2019-12-01
    summary: Allievi Honors Program
  - area: MSc Stochastics and Data Science
    institution: University of Turin
    date_start:  2017-11-01
    date_end: 2019-12-01
    summary: cum laude
  - area: BSc Physics
    institution: University of Turin
    date_start: 2014-09-01
    date_end: 2017-10-01
    summary: cum laude

work:
  - position: Scientist PhD Intern
    company_name: Uber
    company_url: ''
    company_logo: assets/media/uber-logo.svg
    date_start: 2025-06-02
    date_end: 2025-08-22
    summary: |
      PhD Internship on the Membership Science Team at Uber, San Francisco, CA.

      Deployed and refined a membership model by building SQL ingestion pipelines, scaling estimation in PySpark, and delivering automated reporting for stakeholders.
    #  Responsibilities include:
    #  - lorem ipsum dolor sit amet, consectetur adipiscing elit
    #  - lorem ipsum dolor sit amet, consectetur adipiscing elit
    #  - lorem ipsum dolor sit amet, consectetur adipiscing elit
  - position: Risk Analyst Trainee
    company_name: European Central Bank
  #  company_url: ''
    company_logo: assets/media/ecb-logo.svg
    date_start: 2020-01-01
    date_end: 2020-07-31
    summary: |
      Internship in the Risk Analysis Team at the ECB, Frankfurt, Germany.

      Ran daily and weekly monitoring tasks, identified potential flags, and communicated with stakeholders at national central banks.
  #    Responsibilities include:
  #    - Migrated infrastructure to a new data center
  #    - lorem ipsum dolor sit amet, consectetur adipiscing elit
  #    - lorem ipsum dolor sit amet, consectetur adipiscing elit

# Skills
# Add your own SVG icons to `assets/media/icons/`
skills:
  - name: Technical Skills
    items:
      - name: Python
        description: ''
        percent: 80
        #icon: code-bracket
      - name: R
        description: ''
        percent: 100
        #icon: chart-bar
      - name: SQL
        description: ''
        percent: 40
        #icon: circle-stack
  - name: Languages
    color: '#eeac02'
    color_border: '#f0bf23'
    items:
      - name: English
        description: ''
        percent: 60
        #icon: person-simple-walk
      - name: Italian
        description: ''
        percent: 100
        #icon: cat

languages:
  - name: Python
    percent: 90
  - name: R
    percent: 80
  - name: Julia
    percent: 50
  - name: MATLAB
    percent: 50
  - name: C++
    percent: 20
  - name: Java
    percent: 20

#   Awards
#   Add/remove as many awards below as you like.
#   Only `title`, `awarder`, and `date` are required.
#   Begin multi-line `summary` with YAML's `|` or `|2-` multi-line prefix and indent 2 spaces below.
awards:
  - title:
    url: ""
    date: '2020-2025'
    awarder: NYU
    icon: ""
    summary: ""
    url: ""
    date: ""
    awarder: ""
    icon: ""
    summary: ""
---

## About Me

I recently completed a PhD in Economics at New York University, where I worked at the intersection of Economics and Political Science. My research leveraged large-scale text, image, and network data, combining structural modelling and causal inference with machine learning and modern AI. I previously studied Physics, Economics, and Data Science in Turin, Italy.

In Summer 2025, I interned as a Scientist on Uber’s Membership Science team in San Francisco, building and deploying models at scale. I’ll be rejoining the team in Spring 2026.

Feel free to reach out at <code>michele [dot] valinoti [at] gmail [dot] com</code>.

<div class="flex flex-col sm:flex-row gap-4 mt-6">
  <a href="/uploads/Valinoti_Resume_Jan2026.pdf" 
     class="block w-full sm:w-auto px-6 py-4 rounded-lg bg-gray-200 text-black hover:text-green-800 text-center text-lg font-semibold shadow">
    Resume
  </a>
  <a href="/uploads/Valinoti_AcademicCV_Jan26.pdf" 
     class="block w-full sm:w-auto px-6 py-4 rounded-lg bg-gray-200 text-black hover:text-green-800 text-center text-lg font-semibold shadow">
    Academic CV
  </a>
</div>

<style>
  /* Hide Interests & Education grid only in the homepage bio section */
  .blox-resume-biography-3 .grid.grid-cols-1.md\:grid-cols-2 {
    display: none;
  }
</style>