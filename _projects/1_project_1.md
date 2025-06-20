---
layout: page
title: FedBalanceTTA
description: Class Imbalance Mitigation Federated Test-Time Adaptation
img: assets/img/fedbalancett.png
importance: 1
category: Ongoing Research
---

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    <p>
      <strong>FedBalanceTTA: Federated Learning with Balanced Test-Time Adaptation</strong> presents a novel solution to adapt models during inference in federated settings—especially when encountering <em>class imbalance</em> and <em>domain shift</em> in unlabeled test data streams. The framework supports privacy-preserving client-side adaptation without access to ground-truth labels.
    </p>
    <ul>
      <li><strong>Balanced Batch Normalization (BBN):</strong> Computes class-wise normalization statistics from pseudo-labels to mitigate bias toward dominant classes.</li>
      <li><strong>Unsupervised Test-Time Adaptation:</strong> Entropy minimization and confident pseudo-labeling optimize the model during inference.</li>
      <li><strong>Class-Aware Server Aggregation:</strong> Clients are weighted by class distribution skew to preserve minority-class performance during global update.</li>
      <li><strong>Secure Aggregation:</strong> Client updates are privately shared using secure protocols, ensuring privacy of class distributions and raw data.</li>
    </ul>
    <p>
      Extensive experiments on <strong>CIFAR-10-C</strong> and <strong>CIFAR-100-C</strong> benchmarks under multiple corruption and imbalance settings demonstrate that FedBBN outperforms state-of-the-art federated and TTA baselines (e.g., TENT, CoTTA, RoTTA).
    </p>
    <p><strong>📄 Project Paper:</strong> <a href="/assets/pdf/fedbalancetta.pdf" target="_blank">Download PDF</a></p>
  </div>
</div>

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/fedbalancett.png" title="FedBBN: Federated TTA Framework" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

<div class="caption text-center">
  Overview of the proposed FedBBN pipeline showing client-side balanced adaptation, pseudo-label guided normalization, secure aggregation, and class-aware server updates.
</div>

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    <p>
      The framework follows a three-stage process:
    </p>
    <ol>
      <li><strong>Client-Side Adaptation:</strong> Pseudo-labels are generated using the current model; BBN layers normalize features with per-class statistics.</li>
      <li><strong>Secure Aggregation:</strong> Clients encrypt model updates and send them to the server without exposing sensitive distribution or raw data.</li>
      <li><strong>Class-Aware Global Aggregation:</strong> Server aggregates updates using a class-balance-aware weighting to produce a robust, fair global model.</li>
    </ol>
  </div>
</div>

<div class="caption text-center">
  Each client adapts in isolation, and model updates are securely aggregated for bias-free global refinement.
</div>

## 🔖 References

1. Md. Akil Raihan Iftee et al., “FedBalanceTTA – Federated Learning with Balanced Test Time Adaptation,” *ICONIP 2025* (Accepted).
2. Wang et al., “Tent: Fully Test-Time Adaptation by Entropy Minimization,” *ICLR*, 2021.
3. Wang et al., “Continual Test-Time Domain Adaptation,” *CVPR*, 2022.
4. Yuan et al., “Robust Test-Time Adaptation in Dynamic Scenarios,” *CVPR*, 2023.
5. Shao et al., “Federated Face Anti-Spoofing with Test-Time Adaptation,” *FG*, 2021.

---

