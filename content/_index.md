---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Recent Publications
      text: |-
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: experience
    id: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Research engineer
          company: Montefiore Institute, University of Liège
          company_url: ''
          company_logo: 
          location: Liège, Belgium
          date_start: '2018-08-01'
          date_end: ''
          description: |2-
              Research projects with industrial consortia of Belgian companies:
              * IRIS: responsible for the design of environments and algorithms for multi-agent reinforcement learning for decision-aid. 
                Partners: JCD, ACIC, Multitel, ERM.
              * IADAS: responsible for reducing and optimising convolutional neural networks for embedding in drones and satellites.
                Partners: Deltatec, ALX Systems, Spacebel, Multitel.
        - title: Student trainee
          company: X-Ray Imaging Solutions 
          company_url: ''
          company_logo: 
          location: Liege, Belgium
          date_start: '2017-10-01'
          date_end: '2018-07-31'
          description: |2-
              * Development of image processing filters dedicated to X-ray image optimisation.
              * Master thesis: Automatic defect recognition in X-ray imaging by machine learning.

    design:
      columns: '2'
---
