---
layout: page
title: Human Activity Recognition through Wearable Sensor, Video
description: Multimodal Alignment from Video, Sensor(accelerometer, gyroscope, and orientation), Language
img: assets/img/proj10.png
importance: 1
category: Ongoing Research
---

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    <p>
      <strong>Context-Aware Cross-Modal Alignment for Human Activity Recognition</strong> presents a novel multimodal framework for recognizing human activities in complex environments using both visual and wearable sensor data. 
      The system integrates:
    </p>
    <ul>
      <li><strong>Video-LLaVA:</strong> A vision-language model with context prompts for semantic video understanding</li>
      <li><strong>Sensor Features:</strong> Fine-grained motion data from accelerometer, gyroscope, and orientation sensors</li>
      <li><strong>Keyless Attention:</strong> Efficient cross-modal alignment without key-query structures</li>
      <li><strong>Contrastive Learning:</strong> Semantic alignment between modalities using InfoNCE loss</li>
    </ul>
    <p>
      We evaluate on the <strong>MMAct</strong> dataset (27 activities in crowded scenes), demonstrating superior performance over traditional unimodal and fusion baselines. This project combines the semantic richness of large video-language models with the precision of sensor signals to deliver robust human activity understanding.
    </p>
    <p><strong>📄 Project Paper:</strong> <a href="/assets/pdf/har_mmact_.pdf" target="_blank">Download PDF</a></p>
  </div>
</div>

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/proj10.png" title="Proposed HAR Framework" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

<div class="caption text-center">
  Overview of the proposed Human Activity Recognition pipeline using multimodal alignment and contrastive learning.
</div>

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    <p>
      The framework follows a four-stage process:
    </p>
    <ol>
      <li><strong>Feature Extraction:</strong> Video-LLaVA for contextual video embeddings, and 1D CNNs for sensor signals.</li>
      <li><strong>Cross-Modal Alignment:</strong> Keyless attention mechanism computes attention weights over sensor embeddings using video context.</li>
      <li><strong>Joint Fusion & Classification:</strong> Fused representation is passed through a Transformer and MLP for activity classification.</li>
      <li><strong>Loss Optimization:</strong> Combines cross-entropy loss with multimodal contrastive loss for enhanced alignment and generalization.</li>
    </ol>
  </div>
</div>

<div class="caption text-center">
  The training objective combines classification loss and contrastive alignment loss to refine the multimodal representation space.
</div>

## 🔖 References

1. J. Gao et al., “Video-LLaVA: Large Language and Vision Assistant for Video Understanding,” _arXiv:2308.01377_, 2023.
2. Y. Wang et al., “MMAct: A Large-Scale Multi-Modal Dataset for Human Activity Understanding in Crowded Scenarios,” _ICCV_, 2021.
3. X. Chen et al., “Multimodal Sensor Fusion for Human Activity Recognition with Deep Learning,” _IEEE Sensors Journal_, vol. 20, no. 18, pp. 10894–10903, 2020.
4. A. Vaswani et al., “Attention Is All You Need,” _NeurIPS_, 2017.
5. M.-T. Luong et al., “Effective Approaches to Attention-Based Neural Machine Translation,” _arXiv:1508.04025_, 2015.

---
