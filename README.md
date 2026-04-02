# OmniMedHallusion

> Beyond Correct Answers: OmniMedHallusion for Hallucination Analysis in Medical Vision-Language Models

- 🤗 **Hugging Face Dataset**: [OuyangRuilong/OmniMedHallusion](https://huggingface.co/datasets/OuyangRuilong/OmniMedHallusion)

## Overview

OmniMedHallusion is a dataset for hallucination analysis in medical vision-language models.

It contains two complementary subsets:

- **OMH-Clear**: clean medical VQA samples for standard visual understanding
- **OMH-Halluc**: hallucination-oriented samples for robustness analysis

OMH-Halluc includes four clinically motivated settings:

- **CMI**: Cross-Modal Incongruity
- **NOI**: Negative-Option Induction
- **CCA**: Counterfactual Clinical Assumptions
- **PI**: Perceptual Insufficiency

The dataset covers eight imaging modalities and five representative task categories.

## Dataset Comparison

| Dataset | Multimodal | Data Size (k) | Number of (Med-)LVLMs | CMI | NOI | CCA | PI |
|---|---:|---:|---:|---:|---:|---:|---:|
| Med-Halu | ✗ | 2.0 | 3 | ✗ | ✗ | ✗ | ✗ |
| Med-Halt | ✗ | 59.2 | 12 | ✗ | ✓ | ✗ | ✗ |
| CMHE-HD | ✗ | 2.0 | 3 | ✗ | ✗ | ✗ | ✗ |
| CARES | ✓ | 41.0 | 6 | ✗ | ✗ | ✗ | ✓ |
| MedVH | ✓ | 2.0 | 7 | ✓ | ✓ | ✓ | ✗ |
| MedHallVQA | ✓ | 2.3 | 6 | ✓ | ✓ | ✗ | ✗ |
| MedHEval | ✓ | 15.9 | 11 | ✗ | ✗ | ✗ | ✗ |
| Med-HallMark | ✓ | 7.3 | 10 | ✗ | ✗ | ✓ | ✗ |
| MedHallTune | ✓ | 2.2 | 11 | ✗ | ✗ | ✓ | ✗ |
| MedHallBench | ✓ | - | 10 | ✗ | ✗ | ✗ | ✗ |
| **OmniMedHallusion** | **✓** | **131.6** | **33** | **✓** | **✓** | **✓** | **✓** |

## Representative Examples

<p align="center">
  <img src="assets/figure1.png" alt="Representative examples of the four hallucination types in OMH-Halluc" width="900">
</p>

<p align="center">
  <em>Figure 1. Representative examples of the four hallucination types in OMH-Halluc: cross-modal incongruity, negative-option induction, counterfactual clinical assumptions, and perceptual insufficiency.</em>
</p>

## Statistics of OMH-Halluc

<p align="center">
  <img src="assets/figure2.png" alt="Statistics of OMH-Halluc" width="850">
</p>

<p align="center">
  <em>Figure 2. Statistics of OMH-Halluc, including the distribution of hallucination settings, imaging modalities, and task categories.</em>
</p>

## Dataset Statistics

- **Total samples**: 131,662
- **OMH-Clear**: 17,662
- **OMH-Halluc**: 114,000

### Imaging Modalities

- MRI
- Dermoscopy
- Fundus Photography
- Microscopy
- Ultrasound
- OCT
- X-Ray
- CT

### Task Categories

- Disease Diagnosis
- Anatomy Identification
- Modality Recognition
- Biological Attribute Analysis
- Lesion Grading

## Repository Structure

```text
.
├── OMH-Clear/
├── OMH-Halluc/
├── assets/
├── .gitignore
└── compute_metric.ipynb
