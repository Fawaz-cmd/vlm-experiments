# vlm-experiments
Exploring Vision Language Models (VLMs) and multimodal AI workflows using Hugging Face and Google Colab.


# VLM Experiments

This repository contains my experiments and learning journey with Vision Language Models (VLMs) and multimodal AI using Hugging Face and Google Colab.

## Current Work
- BLIP image captioning
- Multimodal inference
- Custom image testing
- Inference parameter experimentation

## Tools & Technologies
- Python
- Hugging Face Transformers
- Google Colab
- PyTorch

## Goal
To explore AI/ML research workflows, understand multimodal models, and gradually move toward advanced VLM and medical AI research.

## Experiments & Observations

### Natural Image Captioning
The BLIP model generated detailed and context-aware captions for common natural images such as sports scenes.

Example:
- Input: Children playing football
- Output: "a painting of children playing soccer in a field"

### Medical-style Image Captioning
The model recognized X-ray style images but produced only high-level captions.

Example:
- Input: Arm X-ray
- Output: "an x-ray of the right arm"

### Observation
The experiments showed that general-purpose VLMs perform better on natural images than specialized medical images, highlighting the importance of domain-specific medical VLMs.

### Model Comparison

BLIP produced more accurate and context-aware captions compared to ViT-GPT2, especially for medical-style X-ray images.

ViT-GPT2 struggled with domain-specific understanding and generated hallucinated outputs such as:
"a black and white photo of a black and white photo of a wall"

This highlighted the importance of domain adaptation and specialized medical VLMs.

## Sample Outputs

### Football Image

Input Image:

![Football Image](football_image.png)

Generated Caption (BLIP):
> "a painting of children playing soccer in a field"

Generated Caption (ViT-GPT2):
> "young men playing a game of soccer"

---

### X-ray Image

Input Image:

![Xray Image](xray_image.png)

Generated Caption (BLIP):
> "an x-ray of the right arm"

Generated Caption (ViT-GPT2):
> "a black and white photo of a black and white photo of a wall"

---

## Observations

- BLIP produced more context-aware captions.
- ViT-GPT2 struggled with medical-style images.
- The experiments highlighted limitations of general-purpose VLMs on specialized medical domains.
