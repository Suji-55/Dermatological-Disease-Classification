# Dermatological Disease Classification Using Machine Learning

## Project Overview

Exploratory machine-learning notebook for classifying six erythemato-squamous skin disorders using clinical and histopathological features. This repository is an **educational, work-in-progress project**, not a medical diagnostic tool.

## Dataset

The notebook describes a dermatology dataset with approximately 366 patient records, 34 input attributes, and six disease classes:

1. Psoriasis
2. Seborrheic dermatitis
3. Lichen planus
4. Pityriasis rosea
5. Chronic dermatitis
6. Pityriasis rubra pilaris

The CSV dataset is **not included**. Obtain the appropriate dermatology dataset from its original provider and update the file path in the notebook.

## Notebook Contents

- Data exploration and class distribution
- Age and symptom analysis
- Correlation and histopathological feature visualizations
- Missing-value and outlier exploration
- Initial train/test split and preprocessing setup

## Repository Structure

```text
Dermatological-Disease-Classification/
├── skin_disorder_project.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## Setup

```bash
python -m venv .venv
# Windows PowerShell
.venv\Scripts\Activate.ps1
pip install -r requirements.txt
jupyter notebook skin_disorder_project.ipynb
```

Update the CSV path in the data-loading cell to point to your local dataset.

## Known Issues / Next Steps

- Normalize `age` / `Age` column naming (cell 42).
- Exclude EDA-only columns such as `Disease_Name` and `Age_Group` from predictors to avoid target leakage (cell 50).
- Fit outlier handling and imputers using training data only.
- Complete model training, validation, evaluation, and reproducible reporting. The uploaded notebook does not yet contain verified final test metrics.

## Disclaimer

For educational purposes only. Do not use this project to diagnose or treat patients. Clinical use requires rigorous external validation, privacy safeguards, and expert oversight.
