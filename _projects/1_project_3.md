---
layout: page
title: Semantic Cognitive Distraction Attack (SCD) in LLM 
description: Multimodal Jailbreak Attack via Contextual Reasoning Manipulation
img: assets/img/scd_attack.png
importance: 1
category: Ongoing Research
---

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    <p>
      <strong>Semantic Cognitive Distraction (SCD)</strong> introduces a novel jailbreak strategy targeting Multimodal Large Language Models (MLLMs). Unlike previous noise-based attacks, SCD exploits models’ contextual reasoning by embedding harmful intent inside a logically consistent and benign narrative.
    </p>
    <ul>
      <li><strong>Contextual Benign Façade:</strong> Embeds harmful goals inside innocuous-sounding prompts (e.g., prop design, educational scenarios).</li>
      <li><strong>Role-Play & Task Priming:</strong> Uses assigned personas (e.g., safety consultant) to anchor intent.</li>
      <li><strong>Visual-Semantic Deception:</strong> Injects payload via disguised images while surrounding them with visually coherent distractors.</li>
      <li><strong>Cognitive Dissonance:</strong> Forces the model to resolve conflicts using its own alignment-breaking reasoning.</li>
    </ul>
    <p>
      We demonstrate this attack against instruction-tuned MLLMs using MM-SafetyBench queries, revealing consistent jailbreak success via carefully staged visual-textual alignment.
    </p>
    <p><strong>📄 Project Paper:</strong> <a href="/assets/pdf/scd_attack_paper.pdf" target="_blank">Download PDF</a></p>
  </div>
</div>

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/scd_attack.png" title="SCD Attack Overview" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

<div class="caption text-center">
  SCD constructs an elaborate but benign-appearing multimodal context that guides the model to process hidden malicious content under plausible intent.
</div>

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    <p><strong>🧠 Attack Pipeline:</strong></p>
    <ol>
      <li><strong>Prompt Engineering:</strong> Embed harmful intent in a role-based instruction (e.g., "You are a prop consultant...").</li>
      <li><strong>Visual Distraction Set:</strong> Compose 3–4 benign support images and 1 payload image disguised with typographic, sketch, or historical aesthetics.</li>
      <li><strong>Task Specification:</strong> Guide the model to sequentially analyze all images and synthesize a step-by-step plan.</li>
      <li><strong>Context Anchoring:</strong> Reinforce benign narrative using references to film, art, or engineering terminology.</li>
    </ol>
  </div>
</div>

<div class="caption text-center">
  The SCD method turns the model’s reasoning alignment into a vulnerability by embedding dangerous payloads inside plausible workflows.
</div>

## 🔖 References

1. D. Yang et al., “CS-DJ: Cognitive Overload Distraction Jailbreak for Multimodal LLMs,” *arXiv:2406.04031*, 2024.  
2. X. Tang et al., “MM-SafetyBench: A Benchmark Suite for Safety Evaluation of Multimodal LLMs,” *arXiv:2403.09792*, 2024.  
3. H. Zhang et al., “HADES: Typographic Attacks for Stealthy Jailbreaks in MLLMs,” *arXiv:2502.10794*, 2024.  
4. OpenAI, “GPT-4 Technical Report,” 2023.  
5. Touvron et al., “LLaVA: Visual Instruction Tuning,” *arXiv:2304.08485*, 2023.

---
