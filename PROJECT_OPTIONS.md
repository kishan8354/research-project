# Research directions

My main focus is hallucination detection and mitigation in vision-language models, especially medical VLMs.

## Visual grounding and hallucination

I want to compare standard decoding with methods that use image evidence more directly. The first step is to run a baseline on a fixed dataset split and examine where its answers go wrong.

Related papers: P01, P03, P04 and P05 in [the reading list](RELATED_PAPERS.md).

Questions I want to study:

- Is the answer supported by the image?
- Does changing or masking the relevant image region change the answer?
- Does a detector use visual evidence, or mainly language and token-position shortcuts?

## Image-text alignment

I want to understand how alignment distillation and preference optimization affect grounding and answer quality.

Related papers: P01 and P02.

## Visual token pruning

I am interested in the trade-off between inference cost, task performance and hallucination when visual tokens are removed.

Related papers: P07 and P08.

## First steps

- Check model and dataset access.
- Run one baseline and record the environment and exact command.
- Use the same examples and settings when comparing methods.
- Record accuracy, hallucination metrics, latency and memory use where relevant.
- Review errors before making changes to the method.
