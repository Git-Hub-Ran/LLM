# Prompt Engineering Experiments

Hands-on experiments showing how prompt phrasing changes the output of
pretrained language models, using Hugging Face Transformers in Google Colab.

## What this covers

**Text generation (GPT-2)** — the same subject is prompted several
different ways to show how framing, specificity, and instruction style
change the continuation the model produces.

**Summarization (BART)** — `facebook/bart-large-cnn` is used to summarize
an article under different instructions, including a length-constrained
"explain it to a child" variant, to compare how constraints affect the
result.

Each experiment is followed by a short written analysis of why the outputs
differ.

## Stack

- Hugging Face Transformers (`pipeline` API)
- `gpt2` for generation, `facebook/bart-large-cnn` for summarization
- PyTorch (as the Transformers backend)
- Google Colab

## Running it

Open the notebook in Google Colab and run the cells top to bottom. No API
key is needed — both models are downloaded from the Hugging Face Hub at
runtime. A GPU runtime is faster but not required.

## Notes

Model outputs are non-deterministic, so re-running the generation cells
will not reproduce the committed outputs exactly. That variability is
part of the point.
