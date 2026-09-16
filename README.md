# multimodal-dual-sentiment

# Multimodal Dual Sentiment Analysis with Custom Class Definitions

This repository contains the code for the Master's thesis:

**"Multimodal Analysis of Expressed and Induced Sentiment 
with Custom Class Definitions"**

*MSc in Data Science and Machine Learning, NTUA, 2025-2026*

## Overview

This thesis investigates the distinction between **expressed sentiment** 
(what the author shows) and **induced sentiment** (what the audience feels) 
in Greek social media posts. Three approaches are evaluated:

- BERT fine-tuning (XLM-RoBERTa, Twitter-XLM-RoBERTa, GreekBERT)
- LLM prompting with custom class definitions (Claude, Llama)
- Multimodal pipeline combining text and image (Claude Vision API)

## Notebooks

| Notebook | Description |
|----------|-------------|
| `thesis_sentiment_colab.ipynb` | BERT fine-tuning experiments (main) |
| `first.ipynb` | LLM prompting + Multimodal pipeline |
| `kwdikas_eda_baseline.ipynb` | Exploratory data analysis |

## Key Results

| Method | Expressed F1 | Induced F1 |
|--------|-------------|------------|
| BERT Fine-tuning | **0.512** | 0.566 |
| Multimodal v1 | 0.353 | 0.567 |
| Multimodal v2 | 0.341 | **0.594** |
| LLM Claude | 0.328 | 0.537 |

## Requirements

```bash
pip install transformers datasets evaluate accelerate
pip install scikit-learn anthropic groq emoji easyocr
```

## Author

Γεωργία Χατζηγιάννη  
National Technical University of Athens  
Supervisor: Γεώργιος Αλεξανδρίδης
