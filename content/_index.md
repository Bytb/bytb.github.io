---
title: ''
summary: 'Caleb Fernandes is a computer science and econometrics student and machine learning researcher at the University of South Florida.'
date: 2026-08-28
type: landing

sections:
  - block: resume-biography-3
    content:
      username: caleb
      text: ''
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: About Me
        education: Education
        interests: Research Interests
    design:
      background:
        gradient_mesh:
          enable: true
      name:
        size: md
      avatar:
        size: medium
        shape: circle
  - block: markdown
    content:
      title: 'Research'
      subtitle: ''
      text: |-
        I work across graph machine learning, causal inference, and spatial computing. My current research includes synthetic electronic health records, feature-free community detection, the local fiscal effects of nuclear development, and disparities in electric-vehicle charging infrastructure.

        My work combines methods from computer science, econometrics, and geographic information systems to study complex systems and build practical analytical tools.
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Publications
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Conferences & Presentations
      filters:
        folders:
          - events
    design:
      view: card
---
