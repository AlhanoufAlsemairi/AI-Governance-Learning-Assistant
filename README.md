# AI Governance Learning Assistant

A domain-specific Large Language Model (LLM) fine-tuned to answer AI Governance questions using Supervised Fine-Tuning (SFT) with LoRA.

## Project Overview

This project demonstrates an end-to-end workflow for adapting an open-source LLM to the AI Governance domain. It covers dataset preparation, fine-tuning, inference, and model evaluation using DeepEval.

## Features

- Fine-tuned Qwen2.5-1.5B-Instruct using LoRA (PEFT)
- Supervised Fine-Tuning (SFT)
- Custom AI Governance Q&A dataset
- Inference pipeline
- Evaluation with DeepEval
- Model Card included

## Tech Stack

- Python
- PyTorch
- Hugging Face Transformers
- TRL
- PEFT
- DeepEval
- OpenRouter (Gemini 3.5 Flash as Judge Model)

## Project Structure

```
AI-Governance-Learning-Assistant/
│
├── notebooks/
│   └── Fine_Tuning.ipynb
├── MODEL_CARD.md
├── README.md
├── requirements.txt
└── data/
```

## Evaluation

| Metric | Value |
|---------|------:|
| Answer Relevancy | 0.82 |
| Pass Rate | 76.19% |
| Test Cases | 21 |

The model was evaluated using DeepEval with Gemini 3.5 Flash as the judge model.

## Future Improvements

- Retrieval-Augmented Generation (RAG)
- Governance Guardrails
- Additional evaluation metrics
- Larger training dataset
- Hallucination detection

## License

This project is intended for educational and research purposes.
