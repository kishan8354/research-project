# Candidate directions — decision pending

These are planning proposals based on the local paper collection. They are not novelty claims and have not been approved by the supervisor.

| Direction | First concrete deliverable | Relevant papers | Main dependency | Later question |
|---|---|---|---|---|
| Evaluate medical VLM hallucinations | Run one baseline on an agreed dataset subset and audit incorrect answers | P01, P03, P04, P05 | Model/data access, inference compute, evaluation labels | Do visual interventions improve grounding beyond language shortcuts? |
| Compare token pruning | Compare a full-token model with one pruning baseline using identical examples and hardware | P07, P08 | Transformer internals and instrumentation | What is the accuracy, hallucination and latency trade-off? |
| Concept-based model debugging | Reproduce a small classification baseline and document concept interventions | P06 | Suitable accessible dataset and concept labels | Which concepts reveal spurious correlations? |

## Select in January 2027

Before committing to a direction, demonstrate that you can explain and run a small PyTorch training loop, handle dataset splits, use Git, read tensor shapes, and record reproducible evaluations. Then assess each option on data access, hardware fit, implementation complexity, supervisor interest and the clarity of the first measurable question.

Training-free methods can still require expensive repeated inference or additional models. Check actual hardware fit rather than assuming they are easy to run. Begin with a baseline before changing the method.
