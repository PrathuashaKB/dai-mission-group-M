# AI-Generated Financial Misinformation: Detection, Market Prediction, and Financial Risk Analysis

![Notebook CI](https://github.com/PrathuashaKB/dai-mission-group-M/actions/workflows/run-notebook.yml/badge.svg)

This project investigates whether advanced machine learning methods can detect AI-generated financial misinformation and whether textual information extracted from financial news contributes to prediction of market outcomes.

The workflow combines:

- Natural Language Processing
- Transformer-based financial sentiment analysis
- Machine Learning classification
- Generative AI robustness evaluation
- Causal analysis of news sentiment and market response

---

## Team

| Name | Role |
|------|------|
| Prathuasha Kandula Bindhu | Lead / Data Collection / Supervised Learning |
| Roshini Venkata Ramana | EDA / Generative AI |
|  Anjali Karna  | Causal Inference |

---

## Research Question

Can advanced machine learning models reliably detect AI-generated financial misinformation, and can textual features extracted from financial news improve prediction of stock market outcomes such as returns, trading volume, and volatility?

---

## Methods Overview

| Block | Method(s) |
|-------|-----------|
| Causal Inference | DoWhy DAG-based analysis and Backdoor Adjustment |
| Supervised Learning | Logistic Regression, Random Forest, Support Vector Machine, Neural Network, FinBERT |
| Generative AI | GPT-4.1-mini based synthetic financial misinformation generation |

---

## Data Sources

| Dataset | Source / URL | Access method |
|---------|-------------|---------------|
| Real Financial News Articles | Reuters and Yahoo Finance | Public financial news sources |
| Financial Market Data | Yahoo Finance using `yfinance` | Runtime download through API |
| Fake and Real News Dataset | Kaggle: https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset | Runtime download using `kagglehub` |
| Synthetic Financial Misinformation Dataset | Generated using GPT-4.1-mini | Generated within project workflow |

> **Data size rule:** Large datasets are not committed to GitHub. Datasets that require external access are downloaded programmatically during execution.

> The Fake and Real News Dataset was initially collected for benchmarking purposes but was not included in the final modelling pipeline. The final analysis focuses on financial-domain data and project-generated synthetic misinformation.

---

## Repository Structure

```
.
├── .github/
│   └── workflows/
│       └── run-notebook.yml
│
├── data/
│   └── processed/
│
├── notebooks/
│   ├── 01_data_collection.ipynb
│   ├── 02_data_cleaning_preparation.ipynb
│   ├── 03_synthetic_generation.ipynb
│   ├── 04_feature_engineering.ipynb
│   ├── 05_detection_models.ipynb
│   ├── 06_robustness_testing.ipynb
│   └── 07_market_prediction.ipynb
│
├── notebook.ipynb
├── presentation.pdf
├── README.md
└── requirements.txt
```

---

## How to Run

### Option A — GitHub Actions

Push to the `main` branch.

The workflow executes `notebook.ipynb` automatically.

Check:

```
GitHub Repository → Actions
```

to verify execution status.

---

### Option B — Local Environment

Clone repository:

```bash
git clone https://github.com/<YOUR_GITHUB_USERNAME>/dai-mission-group-m.git

cd dai-mission-group-m
```

Create environment:

```bash
python -m venv .venv
```

Activate environment:

Windows:

```bash
.venv\Scripts\activate
```

Linux / Mac:

```bash
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run notebook:

```bash
jupyter notebook notebook.ipynb
```

---

## Key Files

| File | Description |
|------|-------------|
| `notebook.ipynb` | Final integrated proposal + analysis notebook |
| `external_notebooks/` | Supporting workflow notebooks |
| `requirements.txt` | Python dependencies |
| `presentation.pdf` | Final presentation slides |

---

## Presentation Slide Requirements

| Item | Rule |
|------|------|
| Content slides | Maximum 5 |
| Allowed extras | Title slide, references, backup slides |
| Required topics | Motivation, Data & Methodology, Results, Limitations & Synthesis |
| File format | PDF only |

---

## Oral Exam

- 15-minute Q&A per group
- Questions cover proposal, methodology, and results
- Each member answers questions related to their assigned block

---

## Submission Checklist

| Item | Status |
|------|--------|
| Repository named `dai-mission-group-m` | ✓ |
| README completed | ✓ |
| Final notebook included | ✓ |
| Notebook executed with outputs visible | ✓ |
| requirements.txt included | ✓ |
| Presentation uploaded as PDF |  |
| External notebooks included | ✓ |
| Large datasets not uploaded directly | ✓ |
| Data downloaded programmatically where required | ✓ |


