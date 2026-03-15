# UWE AI Portfolio: GreenBin Recycling

## Overview

This portfolio contains two AI/ML tasks developed for GreenBin Recycling:

- **Task 1 (NLP):** Customer feedback classification using DistilBERT and RoBERTa transformers
- **Task 2 (Vision):** Waste material recognition using ResNet-18 and ResNet-50 with GradCAM interpretability

## Project Structure

```
├── Task1/
│   └── Task1.ipynb          # NLP pipeline (text classification)
├── Task2/
│   ├── Task2.ipynb          # Vision pipeline (image classification)
│   ├── label_mapping.json   # Class label mapping
│   ├── train_quality_check.csv
│   └── test_quality_check.csv
├── README.md
└── requirements.txt
```

## How to Run

1. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

2. **Hardware:** Both notebooks were developed on a single NVIDIA GPU with 16 GB VRAM. A CUDA-capable GPU is required for training.

3. **Data:** Place the provided training and test data in the respective `Task1/` and `Task2/` directories before running.

4. **Execution:** Open each notebook in Jupyter/VS Code and run cells sequentially. The environment versions cell at the top will confirm your setup matches the development environment.

5. **Model Weights:** Pre-trained `.pth` weight files are available via OneDrive (link provided separately if the zip exceeds the upload limit).

## Key Results

| Task | Model | Accuracy | Macro F1 |
|------|-------|----------|----------|
| Task 1 | Soft-Voting Ensemble (DistilBERT + RoBERTa) | 95.46% | 95.74% |
| Task 2 | Soft-Voting Ensemble (ResNet-18 + ResNet-50 V2) | 95.95% | 95.80% |

## AI Usage Declaration

Generative AI (ChatGPT, Claude, Gemini) was used strictly as a pair-programming assistant for debugging, code review, and optimisation audits. All architectural decisions, model selection, hyperparameter choices, and implementations are the author's own original work. The AI tools were not used to generate answers to the assessment questions or to write the critical evaluation sections.
