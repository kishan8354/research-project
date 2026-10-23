# Related papers

I collect papers here on VLM hallucination, visual grounding and efficient inference. The full catalogue contains dataset, task and metric details.

## Related implementation

[My VGS-Decoding repository](https://github.com/kishan8354/VGS-Decoding) contains an independent implementation of visual-grounding-guided decoding for medical VLMs. It is useful context for comparing the methods below.

## Medical VLM hallucination and grounding

These papers cover medical grounding methods and hallucination evaluation. P05 studies general-domain detectors; its evaluation controls are also relevant when designing medical VLM experiments.

| Paper | Year | Data / dimension | Task and relevance | Code |
|---|---|---|---|---|
| [P01: Enhancing Medical Large Vision-Language Models via Alignment Distillation](https://github.com/Aofei-Chang/MedAlign) | 2026 | MIMIC-CXR; IU-Xray; SLAKE; VQA-RAD; PathVQA; OmniMedVQA; 2D | Medical report generation; Medical VQA. A direct project reference for studying visual grounding through alignment distillation. | [Author link](https://github.com/Aofei-Chang/MedAlign) |
| [P02: Beyond Surface Features: Advancing Medical Vision-Language Alignment via Dynamic Evidence-Guided Preference Optimization](https://aclanthology.org/2026.acl-long.1200/) | 2026 | SLAKE (English subset); VQA-RAD; MIMIC-CXR; IU-Xray; 2D | Medical VQA; Medical report generation. Useful for comparing adaptive preference learning with distillation and inference-time interventions. | Not identified in supplied PDF |
| [P03: Hallucination Detection and Correction in Medical VLMs via Counter-Evidence Verification](https://arxiv.org/abs/2606.18609v1) | 2026 | VQA-RAD; MIMIC-VQA; MIMIC-CXR; IU-Xray; 2D | Medical VQA; Medical report generation; Hallucination detection; Hallucination correction. Relevant to medical visual grounding and inference-time hallucination correction. | Not identified in supplied PDF |
| [P04: Counterfactual Anatomy-guided Spatial-Temporal Decoding for Annotation-Free Hallucination Mitigation in Medical VLMs](https://arxiv.org/abs/2608.17427v1) | 2026 | SLAKE; MIMIC-CXR (VQA formulation); 2D | Medical VQA; Decoding-time hallucination mitigation. A closely related inference-time alternative to CoEV, focused on anatomy-aware decoding. | [Author link](https://github.com/csyifan/CAST) |
| [P05: Robustness of Internal Signals for Hallucination Detection in Vision-Language Models](https://arxiv.org/abs/2610.27041v1) | 2026 | MSCOCO 2014; Objects365 (generalization); 2D | Object hallucination detection in image captions; Robustness and modality sensitivity; Detector ensembling. Motivates token-position and image-ablation controls when evaluating a detector. | Not identified in supplied PDF |

## Visual token efficiency

These papers study visual token pruning. I am interested in how pruning affects hallucination and visual grounding as well as inference cost.

| Paper | Year | Data / dimension | Task and relevance | Code |
|---|---|---|---|---|
| [P07: TransPrune: Token Transition Pruning for Efficient Large Vision-Language Model](https://arxiv.org/abs/2507.20630v2) | 2025 | MME; MMBench; SEED; ScienceQA; VQA-v2; POPE; GQA; TextVQA; TGIF; MSVD; 2D images + video frames | Multimodal perception and reasoning; Image VQA; Video VQA; Efficient inference. A direct reference for a separate efficiency project and possible later grounding–efficiency analysis. | Not identified in supplied PDF |
| [P08: An AI4AI Framework for Visual Token Pruning](https://arxiv.org/abs/2608.07193v2) | 2026 | VQAv2; GQA; VizWiz; ScienceQA-IMG; HallBench; POPE; MME; MMBench-EN; MMBench-CN; MM-Vet; TextVQA; ChartQA; AI2D; OCRBench; 2D | Image VQA; Reasoning; Hallucination evaluation; OCR and chart understanding; Efficient inference. An advanced efficiency reference after understanding deterministic pruning baselines. | [Author link](https://github.com/AIM-ResearchLab/AutoPrune) |

## Alternative and background

P06 covers concept-based model debugging. The surveys and broad benchmark paper provide background on hallucination, post-training and vision evaluation.

| Paper | Year | Data / dimension | Task and relevance | Code |
|---|---|---|---|---|
| [P06: Beyond Explanation: Debugging Medical Imaging Models via Concept Intervention](https://arxiv.org/abs/2610.09031v1) | 2026 | Mayo Clinic ovarian ultrasound dataset; CheXpert 5×200; 2D | Image classification; Concept-based explanation; Model debugging and intervention. Related to causal grounding and interpretability; an alternative project direction. | Not identified in supplied PDF |
| [P09: Understanding Hallucinations in Large Visual and Language Models](https://doi.org/10.1145/3811409) | 2026 | N/A — reviews datasets and studies rather than introducing one experimental dataset; N/A — survey across modalities | Hallucination taxonomy and root-cause survey. Background vocabulary and taxonomy for structuring the survey. | Not identified in supplied PDF |
| [P10: LLM Post-Training: A Deep Dive Into Reasoning Large Language Models](https://doi.org/10.1109/TPAMI.2026.3720414) | 2026 | N/A — survey of post-training literature; benchmarks catalogued in Section V; N/A — primarily text; multimodal coverage | Supervised fine-tuning survey; Preference optimization and RL survey; Test-time scaling survey. Background for understanding DPO, RL and test-time computation before reading DEPO. | [Author link](https://github.com/mbzuai-oryx/Awesome-LLM-Post-training) |
| [P11: Hard Vision, Easy Vision: What GPT-6 Astra Reveals Across Computer Vision](https://arxiv.org/abs/2609.35718v1) | 2026 | 55 benchmarks across 34 capabilities; full benchmark-by-task inventory still to extract; Mixed — 2D, 3D/multiview, video | Recognition and visual reading; Spatial and visual reasoning; 2D grounding and segmentation; 3D perception and geometry; Video understanding; Generation and restoration; Robotics and expert-domain vision. Broad context for task selection; the mixed 3D coverage should not be attributed to the other papers. | [Author link](https://github.com/mbzuai-oryx/frontier-vision) |

