# Negation in Vision-Language Models — Paper List

A curated list of papers on **negation understanding in Vision-Language Models (VLMs)**, organized to accompany the survey:

> **Negation in Vision-Language Models: A Survey**  
> Aashish Pokhrel, Bipin Ghimire, Prashanna Mani Paudel, Shivanand Venkanna Sheshappanavar  
> University of Wyoming  

---

## Table of Contents

- [Survey Paper](#survey-paper)
- [Background: Vision-Language Models](#background-vision-language-models)
- [Background: Negation in NLP](#background-negation-in-nlp)
- [Datasets and Benchmarks](#datasets-and-benchmarks)
  - [Pretraining \& Synthetic Datasets](#pretraining--synthetic-datasets)
  - [Retrieval-Focused Benchmarks](#retrieval-focused-benchmarks)
  - [Diagnostic and VQA Benchmarks](#diagnostic-and-vqa-benchmarks)
  - [Generative and Instruction-Based Benchmarks](#generative-and-instruction-based-benchmarks)
  - [Specialized Domain and Robustness Benchmarks](#specialized-domain-and-robustness-benchmarks)
- [Methods: Data-Centric and Fine-Tuning](#methods-data-centric-and-fine-tuning)
- [Methods: Architectural and Inference-Time](#methods-architectural-and-inference-time)
- [Applications](#applications)
  - [Clinical and Medical Imaging](#clinical-and-medical-imaging)
  - [Image and Video Retrieval](#image-and-video-retrieval)
  - [Generative Models](#generative-models)
- [Related Surveys and Taxonomies](#related-surveys-and-taxonomies)

---

## Survey Paper

| Title | Authors | Venue | Links |
|---|---|---|---|
| Negation in Vision-Language Models: A Survey | Aashish Pokhrel, Bipin Ghimire, Prashanna Mani Paudel, Shivanand Venkanna Sheshappanavar | 2025 | [Paper](#) |

---

## Background: Vision-Language Models

Foundational VLM papers referenced in the survey.

| Title | Authors | Venue | Links |
|---|---|---|---|
| Learning Transferable Visual Models from Natural Language Supervision (CLIP) | Radford et al. | ICML 2021 | [Paper](https://arxiv.org/abs/2103.00020) |
| Visual Instruction Tuning (LLaVA) | Liu et al. | NeurIPS 2023 | [Paper](https://arxiv.org/abs/2304.08485) |
| An Introduction to Vision-Language Modeling | Bordes et al. | arXiv 2024 | [Paper](https://arxiv.org/abs/2405.17247) |
| Vision-Language Models for Vision Tasks: A Survey | Zhang et al. | IEEE TPAMI 2024 | [Paper](https://arxiv.org/abs/2304.00685) |
| Multimodal Fusion and Vision-Language Models: A Survey for Robot Vision | Han et al. | Information Fusion 2025 | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S1566253525007249) |
| Scaling Laws for Native Multimodal Models | Shukor et al. | ICCV 2025 | [Paper](https://openaccess.thecvf.com/content/ICCV2025/html/Shukor_Scaling_Laws_for_Native_Multimodal_Models_ICCV_2025_paper.html) |
| Deep Learning Approaches on Image Captioning: A Review | Ghandi et al. | ACM Computing Surveys 2023 | [Paper](https://arxiv.org/abs/2201.12944) |
| A Decade Survey of Content Based Image Retrieval Using Deep Learning | Dubey | IEEE TCSVT 2021 | [Paper](https://arxiv.org/abs/2012.00641) |
| Renaissance: A Survey into AI Text-to-Image Generation in the Era of Large Model | Bie et al. | IEEE TPAMI 2024 | [Paper](https://ieeexplore.ieee.org/abstract/document/10817489) |

---

## Background: Negation in NLP

Papers on negation understanding in language models.

| Title | Authors | Venue | Links |
|---|---|---|---|
| Say What You Mean! Large Language Models Speak Too Positively about Negative Commonsense Knowledge | Chen et al. | ACL 2023 | [Paper](https://aclanthology.org/2023.acl-long.550/) |
| Can Large Language Models Truly Understand Prompts? A Case Study with Negated Prompts | Jang et al. | TL4NLP @ PMLR 2023 | [Paper](https://arxiv.org/abs/2209.12711) |
| NegBERT: A Transfer Learning Approach for Negation Detection and Scope Resolution | Khandelwal & Sawant | LREC 2020 | [Paper](https://aclanthology.org/2020.lrec-1.704/) |
| Understanding by Understanding Not: Modeling Negation in Language Models | Hosseini et al. | NAACL 2021 | [Paper](https://aclanthology.org/2021.naacl-main.102/) |
| Beyond Positive Scaling: How Negation Impacts Scaling Trends of Language Models | Zhang et al. | ACL Findings 2023 | [Paper](https://aclanthology.org/2023.findings-acl.472/) |
| This is Not Correct! Negation-aware Evaluation of Language Generation Systems | Anschütz et al. | INLG 2023 | [Paper](https://aclanthology.org/2023.inlg-main.12/) |
| Making Language Models Robust Against Negation | Rezaei & Blanco | NAACL 2025 | [Paper](#) |
| NLMS: Augmenting Negation in Language Models | Singh et al. | EMNLP Findings 2023 | [Paper](https://aclanthology.org/2023.findings-emnlp.876/) |
| Strong Hallucinations from Negation and How to Fix Them | Asher & Bhar | ACL Findings 2024 | [Paper](https://aclanthology.org/2024.findings-acl.756/) |
| A Negation Detection Assessment of GPTs: Analysis with the xNot360 Dataset | Nguyen et al. | arXiv 2023 | [Paper](https://arxiv.org/abs/2306.16638) |
| A Multilingual Benchmark for Probing Negation-Awareness with Minimal Pairs | Hartmann et al. | CoNLL 2021 | [Paper](https://aclanthology.org/2021.conll-1.19/) |
| Semantic Inversion, Identical Replies: Revisiting Negation Blindness in Large Language Models | Kim et al. | EMNLP 2025 | [Paper](https://aclanthology.org/2025.emnlp-main.1088/) |
| Thunder-NUBench: A Benchmark for LLMs' Sentence-Level Negation Understanding | So et al. | EACL Findings 2026 | [Paper](https://aclanthology.org/2026.findings-eacl.250/) |
| NUBench: A Benchmark for LLMs' Sentence-Level Negation Understanding | So et al. | — | [Paper](https://openreview.net/forum?id=s7wGbha7dr) |
| Negation: A Pink Elephant in the Large Language Models' Room? | Sojka et al. | arXiv 2025 | [Paper](https://arxiv.org/abs/2503.22395) |
| Investigating and Addressing Hallucinations of LLMs in Tasks Involving Negation | Varshney et al. | TrustNLP 2025 | [Paper](https://aclanthology.org/2025.trustnlp-main.37/) |
| CondaQA: A Contrastive Reading Comprehension Dataset for Reasoning about Negation | Ravichander et al. | EMNLP 2022 | [Paper](https://aclanthology.org/2022.emnlp-main.593/) |
| Generating Diverse Negations from Affirmative Sentences | Vasquez & Papadaki | arXiv 2024 | [Paper](https://arxiv.org/abs/2411.00056) |
| Learning Robust Negation Text Representations | Truong et al. | arXiv 2025 | [Paper](https://arxiv.org/abs/2507.12782) |
| Scale Can't Overcome Pragmatics: The Impact of Reporting Bias on Vision-Language Reasoning | Kamath et al. | arXiv 2026 | [Paper](https://arxiv.org/abs/2602.23351) |
| Towards the Roots of the Negation Problem: A Multilingual NLI Dataset and Model Scaling Analysis | Vrabcová et al. | EMNLP Findings 2025 | [Paper](https://aclanthology.org/anthology-files/pdf/findings/2025.findings-emnlp.1391.pdf) |
| A Comprehensive Taxonomy of Negation for NLP and Neural Retrievers | Petcu et al. | Preprint 2025 | [Paper](https://aclanthology.org/anthology-files/anthology-files/pdf/findings/2025.findings-emnlp.839.pdf) |

---

## Datasets and Benchmarks

### Pretraining & Synthetic Datasets

| Dataset | Task | Size | Paper | Links |
|---|---|---|---|---|
| CC12M | Pre-training | 12.4M image-text pairs (314K negated, 2.53%) | Changpinyo et al., CVPR 2021 | [Paper](https://arxiv.org/abs/2102.08981) |
| LAION-400M | Pre-training | 413.8M pairs (2.4M negated, 0.58%) | Schuhmann et al., arXiv 2021 | [Paper](https://arxiv.org/abs/2111.02114) |
| CC3M | Image Captioning | 3.3M (54K negated train, 1.63%) | Sharma et al., ACL 2018 | [Paper](https://aclanthology.org/P18-1238/) |
| MS-COCO'14 | Image Captioning | 616K captions (1.7K negated train, 0.43%) | Lin et al., ECCV 2014 | [Paper](https://arxiv.org/abs/1405.0312) |
| Flickr30k | Image Captioning | 31K (1.27K negated, 0.04%) | Plummer et al., ICCV 2015 | [Paper](https://arxiv.org/abs/1505.04870) |
| SBU Captions | Image Captioning | 1M (26K negated, 2.62%) | Ordonez et al., NeurIPS 2011 | [Paper](#) |
| CIRR | Composed Image Retrieval | 36K (868 negated train, 3.08%) | Liu et al., ICCV 2021 | [Paper](https://arxiv.org/abs/2105.02987) |
| CC-Neg | Negation understanding (triplets) | 228,246 (image, caption, negated caption) triplets | Singh et al., arXiv 2024 | [Paper](https://arxiv.org/abs/2403.20312) |
| CC12M-NegFull | Fine-tuning negation awareness | 70M+ captions (NegCap + NegMCQ) | Alhamoud et al., CVPR 2025 | [Paper](https://arxiv.org/abs/2501.xxxxx) |
| COVAND | Region-grounded negation detection | 91,110 captions (23,876 images) | Kang et al., arXiv 2025 | [Paper](https://arxiv.org/abs/2510.13232) |
| NeIn (Negative Instruction) | Negation in instruction-based image editing | 366,957 quintuplets | Bui et al., CVPRW 2025 | [Paper](https://openaccess.thecvf.com/content/CVPR2025W/SyntaGen/html/Bui_NeIn_Telling_What_You_Dont_Want_CVPRW_2025_paper.html) |
| HardNeg-Syn | Controlled negation evaluation (image pairs) | 10,000 image pairs | Alhamoud et al., CVPR 2025 | [Paper](https://arxiv.org/abs/2403.20312) |

### Retrieval-Focused Benchmarks

| Benchmark | Task | Size | Paper | Links |
|---|---|---|---|---|
| NegBench (Retrieval) | Inclusion/exclusion retrieval across image, video, medical | 79,239 samples (18 task variations) | Alhamoud et al., CVPR 2025 | [Paper]() |
| NegRefCOCOg | Text-to-image retrieval with negation | 440 triplets | Park et al., 2025 | [Paper](#) |
| nT2VR (Repurposed MSRVTT/VATEX Protocol) | Negation-aware video retrieval | Thousands of negated/composed queries | Wang et al., ACM MM 2022 | [Paper](https://dl.acm.org/doi/10.1145/3503161.3547940) |

### Diagnostic and VQA Benchmarks

| Benchmark | Task | Size | Paper | Links |
|---|---|---|---|---|
| NegBench (MCQ Task) | Fine-grained negation behavior (affirmation, negation, hybrid) | 79,239 samples | Alhamoud et al., CVPR 2025 | [Paper](#) |
| NegVQA | Two-choice QA over objects, attributes, spatial reasoning | 7,379 questions | Zhang et al., ACL Findings 2025 | [Paper](#) |
| NOPE (Negative Object Presence Evaluation) | Object hallucination (absent objects) | 29,500 synthetic NegP samples | Lovenia et al., ALVR Workshop 2024 | [Paper](#) |
| NLVR2 Negation Test Set | Causal mediation analysis of negation | 441 annotated samples | Dobreva & Keller, BlackboxNLP 2021 | [Paper](https://aclanthology.org/2021.blackboxnlp-1.27/) |
| Winoground | Visio-linguistic compositionality | — | Thrush et al., CVPR 2022 | [Paper](https://arxiv.org/abs/2204.03162) |
| ARO (Attribution, Relations, Order) | Compositional understanding | — | Yuksekgonul et al., arXiv 2022 | [Paper](https://arxiv.org/abs/2210.01936) |
| SugarCREPE | VL compositionality (LLM-generated negatives) | — | Hsieh et al., NeurIPS 2023 | [Paper](https://arxiv.org/abs/2306.14610) |
| SNARE | Negation as persistent failure in VL | — | Wang et al., ACM TOMM 2024 | [Paper](#) |
| LogicBench | Logic-focused VL pairs (9 categories, 4 scenarios) | 50,000+ VL pairs | Zhou et al., AAAI 2026 | [Paper](#) |
| Multilingual Negation Benchmark | Cross-linguistic negation (7 languages) | — | Moraitaki et al., arXiv 2026 | [Paper](https://arxiv.org/abs/2604.18942) |
| Text-to-Video Negation Benchmark | Object absence, multi-negation, scope disambiguation | — | Kang & Lin, arXiv 2026 | [Paper](https://arxiv.org/abs/2603.06533) |

### Generative and Instruction-Based Benchmarks

| Benchmark | Task | Size | Paper | Links |
|---|---|---|---|---|
| NEG-TTOI | Negation-aware text-to-image generation accuracy | 2,000 evaluation samples | Cai et al., arXiv 2025 | [Paper](https://arxiv.org/abs/2505.18434) |

### Specialized Domain and Robustness Benchmarks

| Benchmark | Task | Size | Paper | Links |
|---|---|---|---|---|
| CXR-Align | Clinical negation in chest X-ray reports | 3,276 total samples (MIMIC + OpenI) | Ko & Park, CVPR 2025 | [Paper](#) |
| GaslightingBench | Adversarial negation attacks on VLMs | 1,287 samples (20 categories) | Zhu et al., arXiv 2025 | [Paper](#) |

---

## Methods: Data-Centric and Fine-Tuning

### Static Synthetic Negation Datasets with Contrastive / MCQ Objectives

| Method | Base Model | Key Result | Paper | Links |
|---|---|---|---|---|
| NegBench Fine-tuning | CLIP | +10% Retrieval-Neg recall; +28–40% MCQ accuracy | Alhamoud et al., CVPR 2025 | [Paper](#) |
| CoN-CLIP | CLIP | ~99% true-vs-negated on CC-Neg; +4.4% avg R@1 on SugarCREPE | Singh et al., arXiv 2024 | [Paper](https://arxiv.org/abs/2403.20312) |
| NegationCLIP | CLIP (text encoder only) | +9.18 pts on VALSE; +6.36 pts on NegRefCOCOg | Park et al., 2025 | [Paper](#) |
| SemCLIP | CLIP (semantic projection head) | 68.1% → 78.1% orig-over-neg on CC-Neg | Ngan et al., arXiv 2025 | [Paper](https://arxiv.org/abs/2511.16527) |

### Training-Time Dynamic Negation Generation

| Method | Base Model | Key Result | Paper | Links |
|---|---|---|---|---|
| TNG-CLIP | CLIP (text encoder only) | MCQ 81.64% vs CLIP 65.16%; SOTA on NEG-TTOI | Cai et al., arXiv 2025 | [Paper](https://arxiv.org/abs/2505.18434) |

### Task-Specific Negation-Structured Supervision

| Method | Task | Key Result | Paper | Links |
|---|---|---|---|---|
| nT2VR | Text-to-video retrieval | R@1 28.4, R@5 53.7 on MSR-VTT (negated + composed) | Wang et al., ACM MM 2022 | [Paper](https://dl.acm.org/doi/10.1145/3503161.3547940) |
| NeIn | Instruction-based image editing | SOTA editors achieve only 2–8% removal accuracy (first dataset of its kind) | Bui et al., CVPRW 2025 | [Paper](https://openaccess.thecvf.com/content/CVPR2025W/SyntaGen/html/Bui_NeIn_Telling_What_You_Dont_Want_CVPRW_2025_paper.html) |
| CXR-Align | Medical chest X-ray | Adversarial prediction 34.4% (vs baselines 11–23%); strong F1 gains | Ko & Park, CVPR 2025 | [Paper](https://openaccess.thecvf.com/content/CVPR2025/html/Ko_Bringing_CLIP_to_the_Clinic_Dynamic_Soft_Labels_and_Negation-Aware_CVPR_2025_paper.html) |
| CoN2-CLIP | Medical / retrieval | +15% retrieval accuracy on negated/composite prompts | Vu & Sheshappanavar, arXiv 2025 | [Paper](https://arxiv.org/abs/2512.17121) |

### Objective-Centric Reformulation and Logic-Aware Training

| Method | Key Idea | Key Result | Paper | Links |
|---|---|---|---|---|
| Bi-MCQ | Bidirectional MCQ reformulation | Up to 0.47 AUC gains on negation understanding in medical datasets | Kim & Lee, arXiv 2026 | [Paper](https://arxiv.org/abs/2601.22696) |
| LogicCLIP | Logic-aware contrastive training | Gains on LogicBench without sacrificing overall performance | Zhou et al., AAAI 2026 | [Paper](https://ojs.aaai.org/index.php/AAAI/article/view/40143) |

---

## Methods: Architectural and Inference-Time

| Method | Approach | Key Result | Paper | Links |
|---|---|---|---|---|
| NEAT | Test-time adaptation (normalization layers only, no retraining) | +11–14% on Retrieval-Neg + MCQ-Neg; matches fine-tuned SOTA | Han et al., arXiv 2025 | [Paper](https://arxiv.org/abs/2507.19064) |
| SpaceVLM | Training-free geometric subspace modeling | ~30% avg improvement on NegBench (retrieval + MCQ) | Ranjbar et al., arXiv 2025 | [Paper](https://arxiv.org/abs/2511.12331) |
| SpaceVLM-DRC | Training-free query decomposition + dynamic repulsion | COCO Retrieval-Neg R@1 30.2 (+5.2); MSRVTT R@1 28.9 (+5.1) | Pokhrel & Sheshappanavar, CVPRW 2026 | [Paper](#) |
| NEGTOME | Lightweight token-merging + LoRA in cross-attention | Reduces false positives; improves structured detection on COVAND | Kang et al., arXiv 2025 | [Paper](https://arxiv.org/abs/2510.13232) |
| CLIPGLASSES | Plug-and-play dual-stage (Lens + Frame modules, no fine-tuning) | Strong cross-domain generalization | Xiao et al., AAAI 2026 | [Paper](https://ojs.aaai.org/index.php/AAAI/article/view/38075) |
| DEO | Training-free direct embedding optimization via LLM query decomposition | Significant Recall@5 gains on NegConstraint over OpenAI CLIP | Lee et al., arXiv 2026 | [Paper](https://arxiv.org/abs/2603.09185) |
| NEGATE | Negation-derived diffusion guidance constraints (no retraining) | Handles object absence, scope disambiguation, multi-negation in T2V | Kang & Lin, arXiv 2026 | [Paper](https://arxiv.org/abs/2603.06533) |

---

## Applications

### Clinical and Medical Imaging

| Paper | Venue | Links |
|---|---|---|
| Bringing CLIP to the Clinic: Dynamic Soft Labels and Negation-Aware Learning for Medical Analysis (CXR-Align) | CVPR 2025 | [Paper](https://openaccess.thecvf.com/content/CVPR2025/html/Ko_Bringing_CLIP_to_the_Clinic_Dynamic_Soft_Labels_and_Negation-Aware_CVPR_2025_paper.html) |
| The Effect of Negation on CLIP in Medical Imaging: Limitations of Contrastive Language-Image Pretraining (CoN2-CLIP) | arXiv 2025 | [Paper](https://arxiv.org/abs/2512.17121) |
| Bi-MCQ: Reformulating Vision-Language Alignment for Negation Understanding | arXiv 2026 | [Paper](https://arxiv.org/abs/2601.22696) |
| On Large Visual Language Models for Medical Imaging Analysis: An Empirical Study | IEEE CHASE 2024 | [Paper](https://ieeexplore.ieee.org/abstract/document/10614428/) |
| Disparities in Negation Understanding Across Languages in Vision-Language Models | arXiv 2026 | [Paper](https://arxiv.org/abs/2604.18942) |

### Image and Video Retrieval

| Paper | Venue | Links |
|---|---|---|
| Vision-Language Models Do Not Understand Negation (NegBench) | CVPR 2025 | [Paper](https://openaccess.thecvf.com/content/CVPR2025/html/Alhamoud_Vision-Language_Models_Do_Not_Understand_Negation_CVPR_2025_paper.html) |
| Know "No" Better: A Data-Driven Approach for Enhancing Negation Awareness in CLIP (NegationCLIP) | 2025 | [Paper](https://openaccess.thecvf.com/content/ICCV2025/html/Park_Know_No_Better_A_Data-Driven_Approach_for_Enhancing_Negation_Awareness_ICCV_2025_paper.html) |
| Learn to Understand Negation in Video Retrieval (nT2VR) | ACM MM 2022 | [Paper](https://dl.acm.org/doi/abs/10.1145/3503161.3547968) |
| Negation-Aware Test-Time Adaptation for Vision-Language Models (NEAT) | arXiv 2025 | [Paper](https://arxiv.org/abs/2507.19064) |
| SpaceVLM: Sub-Space Modeling of Negation in Vision-Language Models | arXiv 2025 | [Paper](https://arxiv.org/abs/2511.12331) |
| DEO: Training-Free Direct Embedding Optimization for Negation-Aware Retrieval | arXiv 2026 | [Paper](https://arxiv.org/abs/2603.09185) |
| Not Just What's There: Enabling CLIP to Comprehend Negated Visual Descriptions Without Fine-Tuning (CLIPGLASSES) | AAAI 2026 | [Paper](https://ojs.aaai.org/index.php/AAAI/article/view/38075) |

### Generative Models

| Paper | Venue | Links |
|---|---|---|
| TNG-CLIP: Training-Time Negation Data Generation for Negation Awareness of CLIP | arXiv 2025 | [Paper](https://arxiv.org/abs/2505.18434) |
| NeIn: Telling What You Don't Want | CVPR 2025 | [Paper](https://openaccess.thecvf.com/content/CVPR2025W/SyntaGen/html/Bui_NeIn_Telling_What_You_Dont_Want_CVPRW_2025_paper.html) |
| NEGATE: Constrained Semantic Guidance for Linguistic Negation in Text-to-Video Diffusion | arXiv 2026 | [Paper](https://arxiv.org/abs/2603.06533) |
| Negation Blindness in Large Language Models: Unveiling the NO Syndrome in Image Generation | arXiv 2024 | [Paper](https://arxiv.org/abs/2409.00105) |

---

## Related Surveys and Taxonomies

| Title | Authors | Venue | Links |
|---|---|---|---|
| From No to Know: Taxonomy, Challenges, and Opportunities for Negation Understanding in Multimodal Foundation Models | Vatsa et al. | arXiv 2025 | [Paper](https://arxiv.org/abs/2502.09645) |
| Compositionality in Contrastive Vision-Language Models: A Survey of Methods and Benchmarks | Abdolali et al. | 2026 | [Paper](https://www.techrxiv.org/doi/full/10.36227/techrxiv.177004940.09969046/v1) |
| A Survey of Vision-Language Pre-Trained Models | Du et al. | 2022 | [Paper](https://arxiv.org/abs/2202.10936) |
| Explain Before You Answer: A Survey on Compositional Visual Reasoning | Ke et al. | arXiv 2025 | [Paper](https://arxiv.org/abs/2508.17298) |
| From Perception to Cognition: A Survey of Vision-Language Interactive Reasoning in Multimodal Large Language Models | Zhou et al. | arXiv 2025 | [Paper](https://arxiv.org/abs/2509.25373) |
| How and Where Does CLIP Process Negation? | Quantmeyer et al. | ALVR Workshop 2024 | [Paper](https://aclanthology.org/2024.alvr-1.5/) |
| Sparse Visual Thought Circuits in Vision-Language Models | Zhou | arXiv 2026 | [Paper](https://arxiv.org/abs/2603.25075) |
| Polarity-Aware Probing for Quantifying Latent Alignment in Language Models | Sadiekh et al. | AAAI 2026 | [Paper](https://ojs.aaai.org/index.php/AAAI/article/view/41126) |
| Relations, Negations, and Numbers: Looking for Logic in Generative Text-to-Image Models | Conwell et al. | arXiv 2024 | [Paper](https://arxiv.org/abs/2411.17066) |
| Benchmarking Gaslighting Negation Attacks Against Multimodal Large Language Models | Zhu et al. | arXiv 2025 | [Paper](https://ui.adsabs.harvard.edu/abs/2025arXiv250119017Z/abstract) |
| Investigating Negation in Pre-trained Vision-and-Language Models | Dobreva & Keller | BlackboxNLP 2021 | [Paper](https://aclanthology.org/2021.blackboxnlp-1.27/) |
| The Road to Negation: A Comparative Study of Five Typologically and Culturally Diverse Languages | Çabuk-Ballı et al. | First Language 2025 | [Paper](https://journals.sagepub.com/doi/full/10.1177/01427237251336806) |

---

<!-- ## Contributing

If you find a paper on negation in VLMs that is not listed here, feel free to open a pull request with the following format:

```
| Title | Authors | Venue | [Paper](link) |
```

Please make sure the paper is directly relevant to negation understanding in vision-language or multimodal models.

---

## Citation

If you find this list useful, please consider citing our survey:

```bibtex
@article{pokhrel2025negation,
  title={Negation in Vision-Language Models: A Survey},
  author={Pokhrel, Aashish and Ghimire, Bipin and Paudel, Prashanna Mani and Sheshappanavar, Shivanand Venkanna},
  year={2025}
}
``` -->
