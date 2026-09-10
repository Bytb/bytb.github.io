---
title: "Monte Carlo Portfolio Optimization with Downside Risk"
date: "2026-01-01T00:00:00Z"
summary: "Correlated Monte Carlo simulations for portfolio allocation, balancing expected terminal wealth against a 5% conditional-value-at-risk objective."
authors: []
profile: false
tags:
  - Quantitative Finance
featured: false
---

<section class="experience-tools-overview" aria-label="Tools overview">
  <h2>Tools overview</h2>
  <ul>
    <li>Python</li><li>NumPy</li><li>pandas</li><li>SciPy</li><li>Matplotlib</li><li>yfinance</li><li>Quantitative finance</li><li>Monte Carlo simulation</li><li>Portfolio optimization</li><li>Conditional value at risk</li><li>Cholesky decomposition</li><li>Data visualization</li>
  </ul>
</section>

## Select images

<div class="experience-carousel experience-detail-carousel" data-experience-carousel aria-roledescription="carousel" aria-label="Monte Carlo portfolio results">
  <div class="experience-carousel-track">
    <figure class="experience-carousel-slide" aria-hidden="false">
      <img src="/media/projects/monte-carlo/portfolio-paths.png" alt="Simulated portfolio paths from an initial 7000 dollars, with mean terminal wealth of 11250.36 dollars and a fifth-percentile terminal value of 7857.03 dollars">
    </figure>
    <figure class="experience-carousel-slide" aria-hidden="true">
      <img src="/media/projects/monte-carlo/terminal-distribution.png" alt="Distribution of simulated terminal dollar gains, with a mean gain of 4250.36 dollars and a break-even reference at zero" loading="lazy">
    </figure>
  </div>
  <button class="experience-carousel-arrow experience-carousel-prev" type="button" aria-label="Previous image">‹</button>
  <button class="experience-carousel-arrow experience-carousel-next" type="button" aria-label="Next image">›</button>
  <p class="experience-carousel-status" aria-live="polite"></p>
</div>

## Work completed

This project uses correlated Monte Carlo simulations to study portfolio allocation under downside risk. The supplied configuration starts with **$7,000** across **AMZN, CEG, SPYG, and VTI**, estimating asset mean returns and their covariance matrix from historical data.

A Cholesky decomposition transforms independent Gaussian draws into correlated return scenarios. Each scenario compounds weighted daily returns into a portfolio wealth path. During optimization, a fixed set of random draws is reused across candidate allocations so comparisons use the same simulated market scenarios.

The CVaR objective balances expected terminal wealth against a penalty based on the lower 5% tail of terminal wealth. The risk-aversion parameter controls the trade-off between expected wealth and the loss measure derived from conditional value at risk (CVaR). The implementation also supports a Sharpe-ratio objective based on simulated terminal returns. SciPy's SLSQP optimizer enforces a fully invested portfolio and configurable per-asset allocation bounds.

The simulation is vectorized across paths and time steps using NumPy broadcasting and matrix multiplication. After optimization, fresh random draws generate portfolio paths and a distribution of terminal outcomes for the selected weights. Historical adjusted prices are retrieved with yfinance, pandas supports return and risk calculations, and Matplotlib produces the charts.

Reporting includes VaR, CVaR, terminal wealth, probability of profit, and a terminal-return Sharpe ratio. Input diagnostics include annualized return and volatility estimates, dividend yields, and maximum drawdown.

### Illustrated simulation results

- **Mean terminal portfolio value:** $11,250.36.
- **Mean terminal dollar gain:** $4,250.36 relative to the $7,000 starting value.
- **5th-percentile terminal portfolio value:** $7,857.03.

These figures describe the supplied simulation run, not realized investment returns. The 5th-percentile value is a quantile and is distinct from CVaR, which summarizes outcomes in the lower tail. Results depend on the historical mean and covariance estimates and the assumed Gaussian return model.

## GitHub repository

<div class="project-resource-actions">
  <a class="project-resource-button project-resource-github" href="https://github.com/Bytb/Sandbox">View on GitHub →</a>
</div>
