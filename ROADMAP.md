# Work plan

## 1. Read and organize papers

- Review papers on VLM hallucination, visual grounding and medical VQA.
- Record datasets, input types, methods and evaluation metrics.
- Compare the assumptions made by each method.

## 2. Set up a baseline

- Check model, data and GPU requirements.
- Run a small evaluation on a fixed dataset split.
- Save the configuration, command and output.

## 3. Compare methods

- Keep the model, test examples and decoding settings consistent.
- Compare standard decoding with grounding or counterfactual methods.
- Measure answer quality, hallucination and inference cost.

## 4. Review errors

- Look at answers that change under image interventions.
- Check language shortcuts and token-position effects.
- Use the error analysis to decide what to test next.
