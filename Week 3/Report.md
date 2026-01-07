## Week 3 Report – Transformers & Tokenizers

### Goals
- Understand transformer basics (self-attention, encoder/decoder families).
- Try inference with small pretrained models (sentiment, masked LM, text generation).
- Train a custom tokenizer with SentencePiece.
- Build a mini summarization demo with a distilled model.

### What I worked on
- Ran toy self-attention math to see Q/K/V, scores, and weighted outputs.
- Used Hugging Face pipelines: DistilBERT sentiment, DistilRoBERTa fill-mask, DistilGPT2 generation.
- Trained a BPE SentencePiece tokenizer on a slice of WikiText-2; tested encode/decode and reload.
- Mini-project: summarization with `sshleifer/distilbart-cnn-12-6` on CNN/DailyMail samples plus a custom paragraph; measured runtime and compression ratios.

### Key observations
- Pipelines make quick demos easy; small distilled models are fast enough for Colab.
- BPE tokenizer kept vocab small while handling OOV gracefully via subwords.
- DistilBART produced concise summaries; compression ratios showed significant length reduction.

### Files
- Notebooks: `transformer_basics_and_inference.ipynb`, `tokenizer_sentencepiece.ipynb`, `mini_project_summarizer.ipynb`.
- Dependencies: `requirements.txt` (transformers, torch, datasets, sentencepiece).

