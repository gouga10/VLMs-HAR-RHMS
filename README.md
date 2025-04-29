# VLMs-HAR-RHMS
# Keywords Evaluation Notebook

This Jupyter notebook (`Keywords_Evaluate_all_data.ipynb`) is used to evaluate keyword-based generation results across multiple models and datasets. It is intended to support analysis and comparison of different generative models' outputs in terms of alignment with expected or ground-truth captions.

## Overview

The notebook performs the following steps:

1. **Load Model Outputs**: Parses multiple JSON files containing captions or generations from different models:
   - `llama_all.json`: Captions from a LLaMA-based model.
   - `intern2kf.json`: Captions from Intern2K-Finetuned.
   - `internvcaps_toyota.json`: Visual captions from Intern-V.
   - `gpt_toyota_2kf_2.json`: Captions from a GPT-based system.
   - `captions.json`: Ground-truth or human-annotated captions.
   - `dpsk_generations.json`: Outputs from a DPSK model (possibly prompt-guided generations).

2. **DataFrame Creation and Processing**: Each JSON file is loaded and possibly formatted into pandas DataFrames for comparison and analysis.

3. **Evaluation**: Likely includes overlap, matching, or relevance scoring between generated and ground-truth captions using keyword metrics.

## Requirements

- Python 3.8+
- Jupyter Notebook
- Packages:
  - `pandas`
  - `json`

Install requirements via:

```bash
pip install pandas
