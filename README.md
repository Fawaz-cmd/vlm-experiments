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
