# OmniMedHallusion

> Beyond Correct Answers: OmniMedHallusion for Hallucination Analysis in Medical Vision-Language Models

## Overview

OmniMedHallusion is a medical hallucination analysis dataset for vision-language models.

It contains two complementary subsets:

- **OMH-Clear**: clean medical VQA samples for standard visual understanding
- **OMH-Halluc**: hallucination-oriented samples for robustness analysis

OMH-Halluc includes four clinically motivated settings:

- **CMI**: Cross-Modal Incongruity
- **NOI**: Negative-Option Induction
- **CCA**: Counterfactual Clinical Assumptions
- **PI**: Perceptual Insufficiency

## Statistics

- **Total samples**: 131,662
- **OMH-Clear**: 17,662
- **OMH-Halluc**: 114,000
- **Modalities**: MRI, Dermoscopy, Fundus Photography, Microscopy, Ultrasound, OCT, X-Ray, CT
- **Tasks**: Disease Diagnosis, Anatomy Identification, Modality Recognition, Biological Attribute Analysis, Lesion Grading

## Evaluation

OmniMedHallusion supports evaluation from two aspects:

- standard medical visual understanding on **OMH-Clear**
- robustness under hallucination-prone settings on **OMH-Halluc**

We use **OMHScore** to jointly summarize model performance on these two subsets.

## Repository Structure

```text
.
├── OMH-Clear/
├── OMH-Halluc/
├── .gitignore
└── compute_metric.ipynb
