---
layout: page
title: ML/AI Augmented Online Algorithms
description: Making decisions under uncertainty with the help of ML/AI.
img: assets/img/12.jpg
importance: 1
category: research
related_publications: false
---

Learning-Augmented Online Algorithms for Decision-Making Under Uncertainty


Decision-making under uncertainty is fundamental to many real-world systems—from cloud resource provisioning and digital service subscriptions to IoT sensor scheduling and real-time status updating over unreliable wireless channels. In these settings, a decision-maker must act without knowing the future (e.g., future demands, channel states, or time horizons), yet must balance expensive upfront commitments against accumulating ongoing costs. Classical online algorithms provide worst-case performance guarantees (competitive ratios) but are often overly conservative, while machine learning (ML) models trained on historical data deliver strong average-case performance but lack robustness guarantees when facing distribution shifts or adversarial inputs.


To harness the best of both worlds, we develop a unified learning-augmented algorithmic framework that integrates black-box ML predictions into robust online algorithms. The core design principle is a trust-parameterized threshold adjustment: a tunable parameter (θ or λ) controls the degree to which the algorithm trusts the ML prediction. When the prediction suggests a particular action (e.g., purchase, transmit), the algorithm lowers its decision threshold to act sooner; when the prediction suggests inaction, it raises the threshold to delay. This mechanism ensures two provable guarantees simultaneously: (i) consistency—when the ML prediction is accurate, the algorithm closely approximates the optimal offline solution (approaching optimality as trust increases); and (ii) robustness—even when the prediction is arbitrarily inaccurate, the algorithm retains a bounded worst-case competitive ratio (gracefully degrading toward the pure online algorithm as trust decreases). We instantiate this framework across two distinct problem domains—multi-level rent-or-buy decisions and AoI-aware transmission scheduling over ON/OFF channels—and validate through extensive experiments on synthetic and real-world trace data (Azure VM workloads, mobile app usage, mmWave 5G channel measurements) that our algorithms achieve the desired consistency-robustness tradeoff in practice.


Papers (can be found under publication page: [https://zhongdong1994.github.io/publications/](https://zhongdong1994.github.io/publications/)): 
[1] Liu, Zhongdong, et al. "Learning-augmented online minimization of age of information and transmission costs." IEEE Transactions on Network Science and Engineering (2025).
[2] Zhang, Keyuan, et al. "Learning-augmented online algorithm for two-level ski-rental problem." Proceedings of the AAAI Conference on Artificial Intelligence. Vol. 38. No. 18. 2024.
