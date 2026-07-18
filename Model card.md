
## Model Overview

**Model Name:** AI Governance Learning Assistant

**Base Model:** Qwen2.5-1.5B-Instruct

**Fine-tuning Method:** LoRA (PEFT)

**Task:** Domain-specific Question Answering

This model was fine-tuned to answer questions related to AI Governance concepts, including AI risk, fairness, transparency, accountability, privacy, and responsible AI practices.

---

## Intended Use

### Intended Users
- Students
- Researchers
- AI practitioners
- Professionals learning AI Governance

### Intended Use Cases
- Educational AI Governance assistant
- Answering AI Governance questions
- Learning and revision
- Demonstration of LLM fine-tuning

### Out-of-Scope Use
This model should not be used for legal, regulatory, medical, or financial advice, or for high-risk decision-making.

---

## Model Architecture

- Base Model: Qwen2.5-1.5B-Instruct
- Fine-tuning Method: LoRA (PEFT)
- Framework: Hugging Face Transformers
- Trainer: TRL SFTTrainer
- Hardware: NVIDIA Tesla T4 GPU

---

## Training Data

The model was fine-tuned on a custom AI Governance question-answer dataset formatted as instruction-following conversations.

Dataset format:

- User question
- Assistant answer

---

## Fine-tuning Process

- Supervised Fine-Tuning (SFT)
- LoRA adapters
- PEFT
- Hugging Face Transformers
- TRL
- PyTorch

---

## Evaluation

The model was evaluated using DeepEval.

### Evaluation Metric
- Answer Relevancy

### Judge Model
- Google Gemini 3.5 Flash (via OpenRouter)

### Results

- Average Score: **0.82**
- Pass Rate: **76.19%**
- Test Cases: **21**
- Threshold: **0.70**

These results indicate that the model generally produces responses relevant to user questions within the AI Governance domain.

---

## Limitations

- Performance is limited to AI Governance topics.
- The model may generate factually incorrect responses.
- The model does not verify external sources.
- Evaluation used a single metric (Answer Relevancy).

---

## Ethical Considerations

The model is intended for educational purposes only.

Users should verify important information using trusted sources before relying on model outputs.

---

## Risks

Potential risks include:

- Hallucinated information
- Incomplete explanations
- Incorrect interpretation of governance concepts
- Reduced performance on out-of-domain questions

---

## Future Improvements

- Integrate Retrieval-Augmented Generation (RAG)
- Add Governance Guardrails
- Evaluate with additional metrics (Faithfulness, Correctness, Hallucination)
- Expand the training dataset
- Support multilingual AI Governance content

---

## License

This project is intended for educational and research purposes.
