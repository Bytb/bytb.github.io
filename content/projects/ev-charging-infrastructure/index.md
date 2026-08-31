---
title: "EV Charging Infrastructure"
date: "2026-01-01T00:00:00Z"
summary: "Geospatial machine-learning and spatial-accessibility research examining growth and disparities in public EV charging infrastructure across the United States."
authors: []
profile: false
tags:
  - Research
  - Geographic Information Systems
featured: false
---

## Select images

<div class="experience-carousel experience-detail-carousel" data-experience-carousel aria-roledescription="carousel">
  <div class="experience-carousel-track">
    <figure class="experience-carousel-slide" aria-hidden="false">
      <img src="/media/projects/ev-charging-infrastructure/national-road-network.png" alt="National Highway System road network used for EV charging infrastructure analysis">
    </figure>
    <figure class="experience-carousel-slide" aria-hidden="true">
      <img src="/media/projects/ev-charging-infrastructure/prediction-distribution.png" alt="Real and predicted EV charging station counts shown as distributions and a scatter plot" loading="lazy">
    </figure>
    <figure class="experience-carousel-slide" aria-hidden="true">
      <img src="/media/projects/ev-charging-infrastructure/model-metrics.png" alt="Classification and regression evaluation metrics for the EV charging prediction model" loading="lazy">
    </figure>
  </div>
  <button class="experience-carousel-arrow experience-carousel-prev" type="button" aria-label="Previous image">‹</button>
  <button class="experience-carousel-arrow experience-carousel-next" type="button" aria-label="Next image">›</button>
  <p class="experience-carousel-status" aria-live="polite"></p>
</div>

## Project description

This project combines geospatial machine learning and spatial-accessibility analysis to study where public EV charging infrastructure exists, where it is growing, and which communities remain underserved. The modeling pipeline covers **1,048,576 National Highway System road segments** and **83,507 census tracts**, integrating road, demographic, and existing-station features at national scale.

A two-stage LightGBM hurdle model separates the decision into growth classification and positive-growth magnitude. On the held-out test set, the classifier achieved **0.919 AUC** and **0.877 accuracy**. For road segments with positive growth, the regression stage achieved **R² = 0.77**, **RMSE = 12.18**, and **MAE = 8.52**. The predicted-versus-observed plots show that the model captures the overall charging-station growth gradient while retaining the expected difficulty in the sparse, heavy-tailed upper range.

The broader research also includes a Python spatial-accessibility model for county-level public charging access across the United States. A related published offshoot examines spatial disparities in public EV charging infrastructure; it is linked below separately from the core prediction repository.

## GitHub repository

<div class="project-resource-actions">
  <a class="project-resource-button project-resource-github" href="https://github.com/Bytb/EVChargingStationPrediction">View on GitHub →</a>
  <a class="project-resource-button" href="https://www.sciencedirect.com/science/article/pii/S0966692325003989">Read the related publication →</a>
</div>

## Results

The selected figures show the national road-network analysis, predicted versus observed charging-station counts, and the model's classification and regression metrics.
