# 🤖 BERT Question Answering Bot

Welcome to the **QA_WithBERT** project! This repository demonstrates how to build a simple Question Answering (QA) system using 🤗 [Transformers](https://huggingface.co/transformers/) and the **BERT** model fine-tuned on the SQuAD dataset.

## 🔍 Overview

This notebook:
- Loads a pre-trained BERT QA model (`bert-large-uncased-whole-word-masking-finetuned-squad`)
- Uses the tokenizer and model from Hugging Face
- Answers questions based on a given context using PyTorch

## 🧠 Model

The model used:
- **BERT Large Uncased** with whole-word masking
- Fine-tuned on **SQuAD v1.1**

## 📦 Dependencies

Install the required packages with:

```bash
pip install transformers torch
```

## 🛠️ How It Works

1. Load the BERT model and tokenizer
2. Encode a question-context pair
3. Pass it through the model to get start/end logits
4. Decode the answer from the predicted span

## 📗 Example

```python
question = "Who developed BERT?"
context = "BERT was developed by researchers at Google AI Language."
```

The model will return:

```
"researchers at Google AI Language"
```

## 📁 File Structure

- `QA_WithBERT.ipynb` – Jupyter notebook containing the full code and example
- `README.md` – Project overview and instructions

## 📚 References

- [Hugging Face Transformers](https://huggingface.co/transformers/)
- [BERT Paper (Devlin et al., 2018)](https://arxiv.org/abs/1810.04805)

⭐ If you found this useful, feel free to give the repo a star!
