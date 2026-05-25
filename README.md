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



# VLM Experiments

This repository contains my experiments and learning journey with Vision Language Models (VLMs) and multimodal AI using Hugging Face and Google Colab.

---

## Current Work

- BLIP image captioning
- Visual Question Answering (VQA)
- Multimodal inference
- Custom image testing
- Inference parameter experimentation
- Model comparison experiments

---

## Tools & Technologies

- Python
- Hugging Face Transformers
- Google Colab
- PyTorch
- Vision Language Models (VLMs)

---

## Goal

To explore AI/ML research workflows, understand multimodal models, and gradually move toward advanced VLM and medical AI research.

---

# Sample Outputs

## Football Image

Input Image:

![Football Image](football_image.png)

### BLIP Caption
> "a painting of children playing soccer in a field"

### ViT-GPT2 Caption
> "young men playing a game of soccer"

---

## X-ray Image

Input Image:

![Xray Image](xray_image.png)

### BLIP Caption
> "an x-ray of the right arm"

### ViT-GPT2 Caption
> "a black and white photo of a black and white photo of a wall"

---

# Visual Question Answering (VQA)

Explored VQA models using ViLT-based multimodal transformers.

### Example

- Image: Football scene
- Question: "What sport are these children playing?"
- Output: "soccer"

---

# Medical VQA Observations

The VQA model showed strong performance on natural image reasoning tasks but struggled with medical-style X-ray images.

### Examples

- Correctly identified the body part as an arm with low confidence.
- Incorrectly classified the X-ray as non-medical with very high confidence.
- Produced potentially unreliable diagnostic-style answers.

These experiments highlighted hallucination risks and the importance of domain-specific medical VLM finetuning and validation.

---

# Beam Search Experiment

Increasing `num_beams` and `max_new_tokens` improved detail in some cases, but very high values sometimes caused repetitive outputs such as repeated "x-ray" tokens.

This demonstrated generation instability and decoding limitations in smaller VLMs.

---

# Model Comparison

BLIP produced more accurate and context-aware captions compared to ViT-GPT2, especially for medical-style X-ray images.

ViT-GPT2 struggled with domain-specific understanding and generated hallucinated outputs such as:

> "a black and white photo of a black and white photo of a wall"

This highlighted the importance of domain adaptation and specialized medical VLMs.

---

# Key Concepts Explored

- Vision Language Models (VLMs)
- Multimodal AI
- Image Captioning
- Visual Question Answering (VQA)
- Inference
- Beam Search
- Hallucinations in AI
- Domain Adaptation
- Fine-tuning
- Medical AI Limitations

---

# Observations

- General-purpose VLMs perform better on natural images than specialized medical images.
- Different models show different strengths and weaknesses.
- Confidence scores do not always indicate correctness.
- Domain-specific finetuning is important for reliable medical AI systems.

---

# Future Work

- Explore medical-specific VLMs
- Compare additional multimodal models
- Experiment with finetuning concepts
- Study hallucination reduction techniques
- Explore domain-specific AI applications
- Explore advanced medical VQA systems
