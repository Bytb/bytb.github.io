---
title: "Darwin: Portfolio Monitoring and Rebalancing"
date: "2026-01-01T00:00:00Z"
summary: "A React dashboard integrating Schwab account data and market APIs to recommend portfolio rebalancing based on target allocations, contributions, and adjustable RSI influence."
authors: []
profile: false
tags:
  - Quantitative Finance
featured: false
---

<section class="experience-tools-overview" aria-label="Tools overview">
  <h2>Tools overview</h2>
  <ul>
    <li>JavaScript</li><li>React</li><li>Schwab integration</li><li>APIs</li><li>Quantitative finance</li><li>Portfolio rebalancing</li><li>RSI-based allocation</li><li>Data visualization</li>
  </ul>
</section>

## Dashboard

<figure>
  <img src="/media/projects/darwin/rebalance-dashboard.png" alt="Darwin rebalancing dashboard with allocation controls, holdings, purchase recommendations, and portfolio charts, all displaying mock data">
  <figcaption>Darwin portfolio dashboard displaying mock holdings, balances, and performance data for demonstration purposes.</figcaption>
</figure>

## Work completed

Darwin is a portfolio monitoring and rebalancing dashboard built with **JavaScript and React**. It integrates with **Schwab to pull account data** and uses APIs and real market data to generate allocation recommendations. Its rebalancing logic combines target holding percentages with adjustable **Relative Strength Index (RSI)** influence.

### Contribution and cash planning

The dashboard calculates how to distribute a new contribution across holdings to move the portfolio toward its target allocation. Recommendations show dollar amounts, share quantities, and allocation percentages before and after the contribution. It also supports calculating sale amounts to rebalance the account or raise cash. The interface provides recommendations rather than automatically executing trades.

### Configurable allocations

Users can set target weights, minimum shares, maximum allocation per ticker, and the influence of RSI on the rebalancing calculation. Saved configurations support different allocation setups, while selected holdings can be excluded from rebalancing. The allocation overview compares current and effective target weights and identifies overweight and underweight positions.

### Portfolio and market monitoring

Holdings tables bring together shares, market prices, cost basis, market value, unrealized gains and losses, and RSI. Allocation charts compare the current portfolio with the proposed post-contribution allocation. Portfolio performance charts, cash and buying-power summaries, and market-index and VIX panels provide context for reviewing recommendations.
