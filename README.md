# EXIST2025 - Hybrid Sexism Detection System

This repository contains the code, models, and documentation for a hybrid system developed for the EXIST2025 challenge, focused on the detection and analysis of sexism in tweets. The solution integrates fine-tuned transformer models and a hybrid approach with large language models (LLMs) and retrieval-augmented generation (RAG) for robust, explainable predictions.

---

## Project Structure

- `src/notebooks/`: Jupyter notebooks for data processing, model training, evaluation, and hybrid inference.
- `src/data/`: Raw and processed datasets.
- `src/models/`: Saved transformer models and checkpoints.
- `evaluation/`: Scripts and baselines for evaluation and format validation.
- `docs/`: Annotation guidelines and documentation.

---

## Main Features

- **Soft Labels:** Uses annotator vote distributions for robust, subjective label modeling.
- **Advanced Preprocessing:** Emoji normalization, contraction expansion, and multilingual support.
- **Transformers:** Fine-tuned `xlm-roberta-large` for both binary (sexism) and multiclass (intention) tasks.
- **Hybrid System:** Combines transformer predictions with LLM+RAG for explainability and robustness.
- **Evaluation:** Comprehensive metrics (F1, accuracy, ROC-AUC, correlation), visualizations, and error analysis.
- **Export:** Predictions in both CSV and JSON formats, ready for official evaluation.

---

## How to Train

1. **Install dependencies:**
   ```sh
   conda env create -f completeEnv.yml
   conda activate EXIST2025
