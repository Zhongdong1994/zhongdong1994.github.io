---
layout: page
title: Age-of-Information — Freshness–Cost Tradeoffs & Scheduling
description: Update policies and scheduling algorithms that balance information freshness against update cost and service performance.
img: assets/img/3.jpg
importance: 2
category: research
related_publications: false
---

Many real-time services—crowdsensing platforms, monitoring dashboards, and IoT status-update systems—must deliver *fresh* information to users, where freshness is measured by the **Age-of-Information (AoI)**: the time elapsed since the most recently delivered update was generated. Keeping data fresh is not free: it requires frequent updates (incurring energy, bandwidth, or incentive-payment costs) and competes with other work for scarce server capacity. This line of my research characterizes these fundamental tradeoffs and designs provably efficient policies to navigate them.

**Freshness vs. update cost.** For information-update systems where a service provider proactively refreshes its database, I formulated the problem of minimizing the sum of a staleness cost (a function of the AoI) and an update cost as a Markov decision process. I established structural guidelines showing that a simple **threshold-based policy is optimal among all online policies** under Bernoulli request arrivals, derived a closed-form expression for its long-term average cost, and computed the optimal threshold—validated on both synthetic and real traces.

**Freshness vs. service performance and scheduling.** On the scheduling side, I conducted a systematic study of how queueing disciplines affect AoI in single-server queues, showing that leveraging **update-size information** yields large AoI improvements and proving a sample-path equivalence between certain size-based policies (e.g., SRPT) and AoI-based policies. I also studied systems that jointly serve *updates* and *user queries*, proposing threshold policies (Query-k, Update-k, and Joint-(M, N)) that flexibly trade response time against Peak AoI.

Papers (available on the [publications page](https://zhongdong1994.github.io/publications/)):

[1] Liu, Zhongdong, et al. "Toward Optimal Tradeoff Between Data Freshness and Update Cost in Information-Update Systems." *IEEE Internet of Things Journal* 10.16 (2023): 13988–14002. (Conference version: *ICCCN* 2022.)

[2] Liu, Zhongdong, et al. "Anti-Aging Scheduling in Single-Server Queues: A Systematic and Comparative Study." *Journal of Communications and Networks* 23.2 (2021): 91–105. (Conference version: *IEEE INFOCOM Workshops* 2020.)

[3] Liu, Zhongdong, and Bo Ji. "Towards the Tradeoff Between Service Performance and Information Freshness." *IEEE ICC* 2019.
