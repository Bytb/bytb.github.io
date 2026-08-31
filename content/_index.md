---
title: ''
summary: 'Caleb Fernandes is a computer science and econometrics student and machine learning researcher at the University of South Florida.'
date: 2026-08-28
type: landing

sections:
  - block: resume-biography-3
    id: about
    content:
      username: caleb
      text: ''
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: Welcome!
        education: Education
        interests: Research Interests
    design:
      background:
        gradient_mesh:
          enable: false
      name:
        size: md
      avatar:
        size: medium
        shape: circle
  - block: markdown
    id: profile-keywords
    content:
      title: 'Keywords'
      text: |-
        - Machine Learning
        - Neural Networks
        - LLMs
        - Python
        - Data Science
        - Causal Inference
    design:
      columns: '1'
  - block: markdown
    id: highlights
    content:
      title: 'Highlights'
      subtitle: 'Selected honors and research milestones'
      text: |-
        - [**2026 Barry Goldwater Scholar**  
          One of the oldest and most prestigious national undergraduate scholarships in the natural sciences, engineering, and mathematics in the United States.](https://www.usf.edu/ons/news/2026/two-usf-students-named-2026-goldwater-scholars.aspx)

        - [**ICLR 2026 publication**  
          First-authored ReCYCLE Net, published at the GRaM Workshop at ICLR 2026.](/uploads/publications/recycle-net-iclr-2026.pdf)

        - **Award in Economics**  
          Best economics presentation at the 2025 Gulf Coast Undergraduate Research Symposium for research on spatial disparities in U.S. public EV charging infrastructure.

        - **Sigma Xi member**  
          Inducted into the Sigma Xi Scientific Research Honor Society in 2025.

        - **PMEA All-State Band**  
          Second-chair jazz tenor saxophone in the 2021 Pennsylvania Music Educators Association All-State Jazz Band.
    design:
      columns: '1'
  - block: markdown
    id: expertise
    content:
      title: 'Technical Expertise'
      subtitle: 'Methods and tools I use across research and engineering'
      text: |-
        - **Machine Learning** · Graph neural networks, gradient-boosted trees, computer vision, LLMs, synthetic data
        - **Causal & Spatial Methods** · Event studies, panel analysis, time-series analysis, GIS, spatial accessibility
        - **Programming** · Python, SQL, R, C++, C, C#, VBA
        - **Research Stack** · PyTorch, pandas, LightGBM, sf, terra, ggplot2, Unreal Engine 5
    design:
      columns: '1'
  - block: markdown
    id: papers
    content:
      title: Publications
      subtitle: 'Research across graph learning, causal inference, and spatial computing'
      text: |-
        I develop rigorous computational and statistical methods for complex, real-world systems. My current work includes feature-free community detection, synthetic electronic health records, the local fiscal effects of nuclear development, and disparities in electric-vehicle charging infrastructure—combining computer science, econometrics, and geographic information systems from research design through large-scale evaluation.
    design:
      columns: '1'
  - block: collection
    id: published-papers
    content:
      title: 'Published'
      filters:
        folders:
          - publications
        tag: Published
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: working-papers
    content:
      title: 'Working Papers'
      filters:
        folders:
          - publications
        tag: Working Paper
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
  - block: markdown
    id: hobbies
    content:
      title: 'Hobbies'
      subtitle: 'Creative pursuits and interests beyond research'
      text: |-
        - ![Caleb playing saxophone outdoors](hobbies/music.jpeg)

          **Music**

          Saxophone, piano, guitar - its jazz that brings me peace.

        - ![An original coastal painting by Caleb](hobbies/art.jpeg)

          **Art**

          Learned a lot more than just how to oil paint from Bob Ross.

        - ![Caleb studying a financial market chart](hobbies/finance.jpeg)

          **Finance**

          Been in the markets since 2019. Started from fundamental investing and now entirely using quantitative methods.

        - ![Caleb practicing his golf swing](hobbies/golf.jpeg)

          **Golf**

          Somehow the more I practice, the worse I get...
    design:
      columns: '1'
  - block: markdown
    id: projects
    content:
      title: 'Projects'
      subtitle: 'Selected work across quantitative finance and research'
      text: |-
        Explore project pages for descriptions, source-code links, and selected results.
    design:
      columns: '1'
  - block: collection
    id: quant-projects
    content:
      title: 'Quantitative Finance'
      filters:
        folders:
          - projects
        tag: Quantitative Finance
    design:
      view: card
  - block: collection
    id: research-projects
    content:
      title: 'Research'
      filters:
        folders:
          - projects
        tag: Research
    design:
      view: card
---
