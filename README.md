# Vision-Language Hallucination Research

I use this repository to collect papers and notes on hallucination detection and mitigation in vision-language models. My main focus is visual grounding in medical images: whether a model's answer is supported by the image.

I am also looking at image-text alignment, counterfactual decoding and visual token pruning.

## Contents

- [Related papers](RELATED_PAPERS.md)
- [Research directions](PROJECT_OPTIONS.md)
- [Work plan](ROADMAP.md)
- [Experiment template](experiments/TEMPLATE.md)
- [Research notes](meetings/2026-10-23-preparation.md)

## Related implementation

[VGS-Decoding](https://github.com/kishan8354/VGS-Decoding) is my independent implementation of visual-grounding-guided decoding for medical VLMs. I will use the code and its assumptions as a starting point when comparing methods.

## What I want to study

- When a VLM gives an answer that is not supported by the image.
- Whether visual grounding improves answers beyond language-only shortcuts.
- How hallucination, answer quality and inference cost change across methods.

I will record experiment settings, commands and measured results in the experiment notes.

[Full paper collection](https://github.com/kishan8354/survey-paper-collection) · [Daily learning](https://github.com/kishan8354/daily-learning)
