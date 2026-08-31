---
title: "EHR-Walk"
date: "2026-01-01T00:00:00Z"
summary: "A random-walk method for generating synthetic patient data from heterogeneous electronic-health-record graphs."
authors: []
profile: false
tags:
  - Research
  - Synthetic Data
featured: false
---

## Select images

<div class="experience-carousel experience-detail-carousel experience-carousel-landscape" data-experience-carousel aria-roledescription="carousel">
  <div class="experience-carousel-track">
    <figure class="experience-carousel-slide" aria-hidden="false">
      <img src="/media/projects/ehr-walk/ehr-graphs.png" alt="Toy and full heterogeneous electronic health record graph visualizations">
    </figure>
    <figure class="experience-carousel-slide" aria-hidden="true">
      <img src="/media/projects/ehr-walk/wasserstein-ablation.png" alt="Wasserstein distance results across restart probabilities" loading="lazy">
    </figure>
    <figure class="experience-carousel-slide" aria-hidden="true">
      <img src="/media/projects/ehr-walk/provider-exposures.png" alt="Provider degree versus high-risk drug exposure counts" loading="lazy">
    </figure>
    <figure class="experience-carousel-slide" aria-hidden="true">
      <img src="/media/projects/ehr-walk/specialty-transition-heatmap.png" alt="Provider-specialty transition probability heatmap" loading="lazy">
    </figure>
  </div>
  <button class="experience-carousel-arrow experience-carousel-prev" type="button" aria-label="Previous image">‹</button>
  <button class="experience-carousel-arrow experience-carousel-next" type="button" aria-label="Next image">›</button>
  <p class="experience-carousel-status" aria-live="polite"></p>
</div>

## Project description

EHR-Walk is a training-free synthetic-data generator built around random walks on a heterogeneous electronic health record graph. Visits, patients, conditions, drugs, and providers become typed nodes, allowing each synthetic walk to preserve cross-table relationships and multi-valued clinical fields without flattening the EHR into a single independent-and-identically-distributed table. The ablation framework compares directed and undirected graphs, restart probabilities, transition rules, encounter policies, and stopping criteria.

The method generated approximately **45,000 synthetic visits in under two minutes**, compared with roughly 90 minutes of CPU time for GReaT to generate 5,000 visits on the same machine. EHR-Walk synthetic-only training achieved **0.352 macro-F1** for provider-specialty prediction versus a **0.298 real-only baseline**; augmenting real data with EHR-Walk samples increased macro-F1 to **0.441**, a utility ratio of approximately **1.48**. Its p-test AUC of **0.332** and accuracy of **0.393** were also substantially closer to the ideal indistinguishability target of 0.5 than GReaT's 0.996 AUC and 0.985 accuracy.

The companion high-risk-prescribing analysis builds a weighted provider-drug network from standardized OMOP data. After filtering to controlled-substance categories, the final graph connects **2,139 providers** to **123 high-risk drugs** through **4,270 weighted edges**. Personalized PageRank, weighted degree, bipartite density, and square clustering expose specialty-level prescribing structure and flag providers whose exposure volume departs sharply from peers.

Together, the two papers explore a common question: how graph structure can make complex clinical data more useful while keeping the modeling process transparent and computationally efficient. Current limitations include privacy protection, hub-node bias, directed temporal modeling, and sensitivity to graph-construction choices.

## Featured papers

<div class="paper-highlight-grid">
  <a class="paper-highlight-card" href="/uploads/projects/ehr-walk/ehrwalk.pdf">
    <strong>EHRWalk: Synthetic Patient Trajectory Generation Using Heterogeneous Graph Random Walks</strong>
    <span>A graph-based synthetic data generator that uses random walks over heterogeneous EHR structures.</span>
    <em>Read the EHRWalk paper →</em>
  </a>
  <a class="paper-highlight-card" href="/uploads/projects/ehr-walk/abnormal-prescribing-patterns.pdf">
    <strong>Identifying Abnormal Prescribing Patterns in High-Risk Drugs</strong>
    <span>A weighted provider-drug network analysis for identifying prescribing structure and specialty-level outliers.</span>
    <em>Read the network analysis paper →</em>
  </a>
</div>

## GitHub repositories

- [EHR-Walk synthetic data synthesis](https://github.com/Bytb/EHR_RandomWalk_SynethticDataSynthesis)
- [High-risk prescribing network analysis](https://github.com/Bytb/EHRShot_Project)
