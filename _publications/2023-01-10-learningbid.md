---
title: "Analysis of a Learning Based Algorithm for Budget Pacing"
collection: publications
permalink: /publication/2023-01-10-learningbid
excerpt: 
date: 2023-01-10
venue: 'AAMAS'
paperurl: 
citation: 'MohammadTaghi Hajiaghayi and Max Springer.  (2022).  &quot;Analysis of a Learning Based Algorithm for Budget Pacing&quot;  (AAMAS 2023)'
---

In this paper, we analyze a natural learning algorithm for uniform pacing of advertising budgets, equipped to adapt to varying ad sale platform conditions. On the demand side, advertisers face a fundamental technical challenge in automating bidding in a way that spreads their allotted budget across a given campaign subject to hidden, and potentially dynamic, cost functions. This automation and calculation must be done in runtime, implying a necessarily low computational cost for the high frequency auction rate. Advertisers are additionally expected to exhaust nearly all of their sub-interval (by the hour or minute) budgets to maintain budgeting quotas in the long run. To resolve this challenge, our study analyzes a simple learning algorithm that adapts to the latent cost function of the market and learns the optimal average bidding value for a period of auctions in a small fraction of the total campaign time, allowing for smooth budget pacing in real-time. We prove our algorithm is robust to changes in the auction mechanism, and exhibits a fast convergence to a stable average bidding strategy. The algorithm not only guarantees that budgets are nearly spent in their entirety, but also smoothly paces bidding to prevent early exit from the campaign and a loss of the opportunity to bid on potentially lucrative impressions later in the period. 

In addition to the theoretical guarantees, we validate our algorithm with experimental results from open source data on real advertising campaigns to further demonstrate the effectiveness of our proposed approach.

[Download paper here](https://arxiv.org/pdf/2205.13330.pdf)
