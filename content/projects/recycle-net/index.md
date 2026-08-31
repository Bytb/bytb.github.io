---
title: "ReCYCLE Net"
date: "2026-04-26T00:00:00Z"
summary: "A feature-free, unsupervised graph neural network for community detection using renewal non-backtracking random-walk cycle information and graph attention."
authors: []
profile: false
tags:
  - Research
  - Graph Machine Learning
featured: false
---

## Select images

<div class="experience-carousel experience-detail-carousel" data-experience-carousel aria-roledescription="carousel">
  <div class="experience-carousel-track">
    <figure class="experience-carousel-slide" aria-hidden="false">
      <img src="/media/projects/recycle-net/poster-presentation.jpeg" alt="Caleb Fernandes presenting the ReCYCLE Net poster at ICLR">
    </figure>
    <figure class="experience-carousel-slide" aria-hidden="true">
      <img src="/media/projects/recycle-net/iclr-portrait.jpeg" alt="Caleb Fernandes at the ICLR conference" loading="lazy">
    </figure>
    <figure class="experience-carousel-slide" aria-hidden="true">
      <img src="/media/projects/recycle-net/conference-hall.jpeg" alt="ICLR conference exhibition hall" loading="lazy">
    </figure>
    <figure class="experience-carousel-slide" aria-hidden="true">
      <img src="/media/projects/recycle-net/rio-christ-redeemer.jpeg" alt="Caleb Fernandes visiting Christ the Redeemer in Rio de Janeiro" loading="lazy">
    </figure>
  </div>
  <button class="experience-carousel-arrow experience-carousel-prev" type="button" aria-label="Previous image">‹</button>
  <button class="experience-carousel-arrow experience-carousel-next" type="button" aria-label="Next image">›</button>
  <p class="experience-carousel-status" aria-live="polite"></p>
</div>

## Project description

ReCYCLE Net (RCN) is a feature-free, cycle-aware graph neural network for unsupervised community detection. It converts Renewal Non-Backtracking Random Walk retrace probabilities into edge-reinforcement weights and injects that cycle signal into a Graph Attention Network. The model learns node embeddings through a combined objective covering modularity, Laplacian smoothness, contrastive consistency, and orthogonality, then extracts communities with clustering.

The project evaluates whether explicit cycle structure improves community recovery across social, citation, and protein-interaction graphs. RCN reached **0.60 NMI and 0.67 ARI on PolBooks**, a **0.85 Facebook silhouette score**, and **0.344 overlap NMI on Complex Portal at two memberships per node**. On the overlapping protein-complex benchmark, that ONMI exceeded the reported generative, attention, and modularity baselines of 0.243, 0.232, and 0.140. Results were strongest in cycle-rich graphs, while performance remained competitive when cyclic closure was weaker.

### Technical scale

- Evaluated graphs as large as 56,944 nodes.
- Combined cycle-aware attention with a fully unsupervised multi-term loss.
- Tested structural and ground-truth community counts, overlapping memberships, ablations, rewired graphs, and multiple random seeds.
- First-authored work published in the GRaM Workshop proceedings at ICLR 2026.

## GitHub repository

<div class="project-resource-actions">
  <a class="project-resource-button project-resource-github" href="https://github.com/Bytb/RCN">View on GitHub →</a>
  <a class="project-resource-button" href="/uploads/publications/recycle-net-iclr-2026.pdf">Open the paper →</a>
</div>
