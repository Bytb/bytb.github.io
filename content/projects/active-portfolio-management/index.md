---
title: "Value and Momentum: From Signals to Factor Forecasts"
date: "2026-01-01T00:00:00Z"
summary: "A hands-on study motivated by Active Portfolio Management by Richard Grinold and Ronald Kahn, practicing forecasting techniques with momentum and price-based value signals."
authors: []
profile: false
tags:
  - Quantitative Finance
featured: false
---

<section class="experience-tools-overview" aria-label="Tools overview">
  <h2>Tools overview</h2>
  <ul>
    <li>Python</li><li>NumPy</li><li>pandas</li><li>SciPy</li><li>statsmodels</li><li>Matplotlib</li><li>yfinance</li><li>Jupyter Notebook</li><li>Quantitative finance</li><li>Factor modeling</li><li>Regression</li><li>Bayesian shrinkage</li><li>Time-series analysis</li><li>Data visualization</li>
  </ul>
</section>

## Select images

<div class="experience-carousel experience-detail-carousel" data-experience-carousel aria-roledescription="carousel" aria-label="Value and momentum results">
  <div class="experience-carousel-track">
    <figure class="experience-carousel-slide" aria-hidden="false">
      <img src="/media/projects/value-and-momentum/information-decay.png" alt="Mean Spearman information coefficients for momentum and value across forecast horizons of one to twelve months, with error bars">
    </figure>
    <figure class="experience-carousel-slide" aria-hidden="true">
      <img src="/media/projects/value-and-momentum/factor-returns.png" alt="Scatter plot of momentum versus value factor returns showing a negative relationship" loading="lazy">
    </figure>
    <figure class="experience-carousel-slide" aria-hidden="true">
      <img src="/media/projects/value-and-momentum/cumulative-performance.png" alt="Cumulative momentum and value factor performance from 2010 through 2025, expressed as growth of one dollar" loading="lazy">
    </figure>
  </div>
  <button class="experience-carousel-arrow experience-carousel-prev" type="button" aria-label="Previous image">‹</button>
  <button class="experience-carousel-arrow experience-carousel-next" type="button" aria-label="Next image">›</button>
  <p class="experience-carousel-status" aria-live="polite"></p>
</div>

## Work completed

This project is motivated by *Active Portfolio Management* by **Richard Grinold and Ronald Kahn** and is intended as hands-on practice with the techniques presented in the book. It connects equity prices, stock-level signals, information coefficients, and factor returns. The study uses monthly observations from **2010–2025**, a fixed universe of U.S. equities, and **SPY** as the market benchmark, with additional history for long-lookback signals.

Momentum measures returns from months **t−12 through t−2**, excluding the most recent month to separate medium-term continuation from short-term reversal. Price-based value uses the negative of the trailing **60-month return** as a long-term reversal proxy. Both signals are standardized across stocks each month.

The analysis decomposes stock returns relative to SPY and tests whether residual return volatility is embedded in signal volatility. Monthly information coefficients measure the relationship between each signal and subsequent residual returns; the forecasting framework also considers estimation uncertainty and Bayesian shrinkage.

Long–short factor portfolios use the previous month's signal rankings, buying the highest-scoring tercile and shorting the lowest-scoring tercile. Their returns are evaluated using the following month's realized residual returns.

### Selected findings

- Momentum produced a small positive average monthly factor return, but the estimate was not statistically distinguishable from zero.
- The price-based value factor had a negative average monthly return, performing opposite to its intended reversal interpretation over this sample.
- Momentum and value factor returns had a correlation of approximately **−0.435**. Their regression relationship was statistically significant, with **R² ≈ 0.189**, leaving substantial independent variation.

### Signal persistence and forecasting horizon

The next stage distinguishes persistence in signal scores from persistence in their predictive information. It examines forward information coefficients at increasing horizons, tests an exponential information-decay model, and translates decay into an information half-life where that model is appropriate. Comparing score persistence with information decay helps assess whether older signals add useful information beyond the latest observation.

The broader objective is to extend this analysis to multifactor forecasts and stock-level return forecasts using factor correlations and estimated stock exposures.

### Study design

The fixed universe is selected from companies known today and requires sufficient historical data, introducing **survivorship bias**. This is a study of forecasting methodology rather than a production-quality historical trading strategy. The value signal is a price-only reversal proxy, not a valuation measure based on company fundamentals.

## GitHub repository

<div class="project-resource-actions">
  <a class="project-resource-button project-resource-github" href="https://github.com/Bytb/Sandbox">View on GitHub →</a>
</div>
