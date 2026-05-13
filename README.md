# Arabic-Poetry-FineTuning
# Arabic Poetic Reasoning

Arabic AI project for generating suitable Arabic poetic verses based on semantic scenarios using NLP and Large Language Models (LLMs).

---

## Project Overview

This project builds an Arabic AI system capable of understanding a written situation or emotional scenario and generating an appropriate Arabic poetic verse that reflects the meaning.

The project combines:
- Arabic NLP
- Semantic Reasoning
- Text Generation
- Fine-Tuning LLMs

---

## Project Pipeline

### 1. Poetry Extraction
Poetic texts were extracted from PDF files and converted into machine-readable text files.

### 2. Dataset Construction
A custom JSON dataset was created in the following format:

```json
{
  "input": "scenario",
  "output": "poetic verse"
}
```

### 3. Data Preparation
The dataset was transformed into conversational format suitable for instruction-tuned language models.

### 4. Model Fine-Tuning
The model was fine-tuned using:
- Unsloth
- LoRA
- 4-bit Quantization
- Gradient Checkpointing

### 5. Inference & Testing
The trained model was evaluated on unseen scenarios to test semantic understanding and poetic generation quality.

---

## Technologies Used

- Python
- Google Colab
- Qwen3-4B-Instruct
- Unsloth
- PyTorch
- Hugging Face Transformers
- TRL
- Datasets
- Gemini API
- Groq API
- JSON

---

## Model Information

Base Model:
- Qwen3-4B-Instruct

Training Framework:
- Unsloth

Optimization Techniques:
- LoRA Fine-Tuning
- 4-bit Quantization
- Gradient Checkpointing
- Response-Only Training

---

## Example

### Input
```text
إذا رأى من أخلف وعده
```

### Output
```text
بيت شعري مناسب للموقف
```

---

## Training Configuration

| Parameter | Value |
|---|---|
| Batch Size | 2 |
| Gradient Accumulation | 4 |
| Epochs | 3 |
| Learning Rate | 2e-4 |
| Optimizer | AdamW 8-bit |

---

## Features

- Arabic poetic reasoning
- Scenario-to-poetry generation
- Semantic understanding
- Memory-efficient fine-tuning
- Arabic text generation

---

## Challenges

- Limited Arabic datasets
- High memory consumption
- Hallucination in text generation

---

## Future Improvements

- Expand dataset size
- Use larger language models
- Add BLEU / ROUGE evaluation
- Integrate RAG systems
- Build a user interface

---

## Files

### `final_project1.py`
Responsible for:
- Reading text files
- Extracting scenarios and poetic verses
- Building the JSON dataset

### `fainal_project2.py`
Responsible for:
- Loading the model
- Fine-tuning using Unsloth
- Training and testing the model
- Saving the trained model

---

## Author

Nourh Turki Alajalein

Arabic NLP Bootcamp — SDAIA

---

## License

This project is for educational and research purposes.
