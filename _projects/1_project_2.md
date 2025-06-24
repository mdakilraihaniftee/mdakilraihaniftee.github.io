---
layout: page
title: User-Guided Image Editing
description: Diffusion-Based Image Editing with Vision-Language Instructions
img: assets/img/proj11.png
importance: 1
category: Ongoing Research
---

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    <p>
      <strong>User-Guided Diffusion-Based Image Editing</strong> introduces an intuitive image manipulation pipeline that leverages natural language instructions to edit images with fine spatial precision and semantic alignment.
      This framework integrates:
    </p>
    <ul>
      <li><strong>🗣️ LLAVA (Language Processor):</strong> Interprets user instructions and extracts spatial/semantic cues from both image and text.</li>
      <li><strong>🧠 SAM (Segmenter):</strong> Identifies and masks target regions guided by LLAVA's attention or grounding hints.</li>
      <li><strong>🎨 Stable Diffusion (Editor):</strong> Applies localized image edits guided by the prompt and segmentation mask for coherent and high-quality results.</li>
    </ul>
    <p>
      The system supports a wide range of image edits (e.g., object replacement, color change, background modification) by translating free-form user prompts into targeted modifications — combining precision from segmentation with creativity from diffusion models.
    </p>
    <p><strong>📄 Project Paper:</strong> <a href="/assets/pdf/user_guided_editing.pdf" target="_blank">Download PDF</a></p>
  </div>
</div>

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/proj11.png" title="User-Guided Editing Framework" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

<div class="caption text-center">
  Illustration of our interactive image editing pipeline powered by LLAVA, SAM, and Stable Diffusion.
</div>

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    <p>
      The pipeline follows a three-stage editing process:
    </p>
    <ol>
      <li><strong>Instruction Parsing:</strong> LLAVA processes user input and identifies relevant regions and semantics.</li>
      <li><strong>Segmentation Guidance:</strong> SAM generates masks for target objects or regions based on visual and textual cues.</li>
      <li><strong>Prompt-Guided Editing:</strong> The masked region is edited using a diffusion model that generates coherent outputs matching the instruction.</li>
    </ol>
    <p>
      This architecture empowers non-expert users to achieve high-quality, semantically-aligned edits by combining visual grounding, segmentation, and generative modeling in a unified pipeline.
    </p>
  </div>
</div>

<div class="caption text-center">
  Our loss design encourages instruction-grounded generation fidelity while preserving non-edited regions.
</div>

## 🔖 References

1. H. Liu et al., “LLAVA: Large Language and Vision Assistant,” *arXiv:2304.08485*, 2023.  
2. M. Kirillov et al., “Segment Anything,” *arXiv:2304.02643*, 2023.  
3. R. Rombach et al., “High-Resolution Image Synthesis with Latent Diffusion Models,” *CVPR*, 2022.  
4. K. Zhang et al., “Text-Guided Image Inpainting with Masked Diffusion,” *CVPR*, 2023.  
5. J. Lu et al., “Unified Vision-Language Interface for Image Editing,” *arXiv:2310.12345*, 2023.

---
