---
layout: page
title: Age-of-Information — Robust Analysis & Pull-Model Learning
description: New analytical tools (robust queueing) and learning-based methods for characterizing and optimizing information freshness.
img: assets/img/7.jpg
importance: 3
category: research
related_publications: false
---

Beyond designing update and scheduling policies, my research develops new *analytical* and *learning-based* tools for Age-of-Information (AoI). Classical AoI analysis relies on probabilistic assumptions (e.g., memoryless or i.i.d. arrivals) that break down for the heavy-tailed and correlated traffic seen in practice; and in many modern applications the freshness-optimal action must be *learned* online rather than computed from a known model.

**Robust-queueing analysis of AoI.** I introduced a robust-optimization approach to bound the **Peak AoI (PAoI)**: instead of assuming a specific distribution, I model the uncertainty in the arrival and service processes with *uncertainty sets*, yielding worst-case PAoI approximations for very general (including heavy-tailed and correlated) processes. Unlike classical bounds (e.g., Kingman-type bounds under i.i.d. assumptions) that are loose under light load, the resulting approximation is accurate across both light and high load—the two regimes most critical for AoI.

**Freshness under the Pull model with learning.** I also studied a *Pull model* in which a user proactively sends replicated requests to multiple servers to fetch fresh information. Replication exposes a novel tradeoff between the differing AoI values and response times across servers; I derived the optimal number of responses to wait for and showed that—perhaps counterintuitively—**waiting for more than one response often reduces AoI**. When the system is unknown, I reformulated freshness (utility) maximization as a stochastic multi-armed bandit with side observations and designed learning algorithms with improved performance guarantees.

Papers (available on the [publications page](https://zhongdong1994.github.io/publications/)):

[1] Liu, Zhongdong, et al. "A Worst-Case Approximate Analysis of Peak Age-of-Information Via Robust Queueing Approach." *IEEE INFOCOM* 2021.

[2] Li, Fengjiao, Yu Sang, Zhongdong Liu, et al. "Waiting But Not Aging: Optimizing Information Freshness Under the Pull Model." *IEEE/ACM Transactions on Networking* 29.1 (2021): 465–478.
