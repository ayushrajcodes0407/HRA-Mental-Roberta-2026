# Hierarchical Mental Health Text Classification
This is the implementation/codebase of our attached research work. 
"Hierarchical Risk-Aware Mental-RoBERTa Framework for Early Multi-Class
Screening of Mental-Health Conditions and Suicidal Ideation, 2026" by Ayush Raj, Abhinav Srivastava, Dr. Kamnta Nath Mishra and Dr. Alok Mishra

Implementation of a hierarchical transformer-based framework for multi-class mental health text classification.
Author: Ayush Raj
Collaborator: Abhinav Srivastava

The system decomposes the task into two stages:

- **Stage 1** performs binary classification to distinguish Normal and At-Risk samples.
- **Stage 2** classifies only At-Risk samples into the corresponding mental health categories.

A rule-based decision layer is applied after Stage-2 to improve prediction consistency for clinically important classes.

---

## Repository Structure

```
notebook/
    main.ipynb

models/
├── stage-1/
│   └── drive/
│       └── MyDrive/
│           └── mental_health_project/
│               └── stage1_model/
│                   ├── config.json
│                   ├── merges.txt
│                   ├── model.safetensors
│                   ├── special_tokens_map.json
│                   ├── tokenizer.json
│                   ├── tokenizer_config.json
│                   ├── training_args.bin
│                   └── vocab.json
│
└── stage-2/
    └── drive/
        └── MyDrive/
            └── mental_health_project/
                └── stage2_model/
                    ├── config.json
                    ├── merges.txt
                    ├── model.safetensors
                    ├── special_tokens_map.json
                    ├── tokenizer.json
                    ├── tokenizer_config.json
                    ├── training_args.bin
                    └── vocab.json

data/
    data.md

---
```
## Pipeline

```
Input Text
      │
      ▼
Stage-1 Binary Classifier
      │
 ┌────┴────┐
 │         │
Normal   At-Risk
             │
             ▼
 Stage-2 Multi-class Classifier
             │
             ▼
 Rule-based Decision Layer
             │
             ▼
 Final Prediction
```

---

## Training
```
Train Stage-1 first.

The trained Stage-1 model is then used to identify At-Risk samples for Stage-2 training.

---
```
## Evaluation
```
The repository includes:

- Classification accuracy
- Macro F1-score
- Confusion matrices
- Bootstrap confidence intervals
- Generalization gap analysis
- Flat classifier baseline comparison
```
---

## Models
```
The implementation uses:

- RoBERTa encoder
- Weighted loss for class imbalance
- Hierarchical classification
- Rule-based post-processing
```
---

## Outputs
```
The evaluation produces:

- Classification reports
- Confusion matrices
- Statistical analysis
- Learning curves
- Bootstrap confidence intervals
```

---

## Citation

If this repository is used in academic work, please cite the associated paper.
