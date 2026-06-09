---
layout: page
title: project Matryoshka
description: My first project at Meta
img: assets/img/12.jpg
importance: 1
category: work
related_publications: true
---

Over the past decade, data center networking (DCN) has undergone substantial transformation in terms of both scale and complexity. Developing a DCN entails multiple intricate steps, such as establishing physical connections, configuring logical network addressing, and defining high-level routing policies. While extensive work has focused on logical DCN design and physical deployment, a critical gap remains: materializing these designs into concrete switch configurations—a necessary step to realize the development procedure. This problem is especially acute in the AI era, as hyperscale, rapidly evolving, and highly heterogeneous AI-driven clusters place unprecedented demands on DCN design and implementation.

Matryoshka, Meta’s production-scale DCN design system that bridges this gap. Matryoshka employs an intent-based, model-driven approach to systematically compile high-level DCN design intents into working switch configurations. Operational for over six years, Matryoshka has supported orders-of-magnitude growth in Meta’s DCN infrastructure, guiding the design nearly 900 DCNs across 18 distinct types, including the latest 100K-GPU supercluster for AI training. We share our experience in building and operating Matryoshka, highlighting how it empowers the rapid design and evolution of AI clusters nowadays.

Team paper (published before I joined the team): [Cai, Yan, et al. "Matryoshka: Realizing Hyperscale Data Center Network Design for the {AI} Era." 23rd USENIX Symposium on Networked Systems Design and Implementation (NSDI 26). 2026.](https://www.usenix.org/conference/nsdi26/presentation/cai) 

Presentation link: [https://www.youtube.com/watch?v=e8St497tql8&t=21s](https://www.youtube.com/watch?v=e8St497tql8&t=21s)
