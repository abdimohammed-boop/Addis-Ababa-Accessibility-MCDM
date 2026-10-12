# MCA–TOPSIS Road Accessibility Evaluation

This repository provides open-access field audit datasets, processed PwDs survey responses, and Python calculation scripts for evaluating pedestrian road accessibility along arterial corridors connecting to Addis Ababa.

## Data Files (`/data`)
* `raw_field_audit_5corridors.csv`: Physical measurements across 9 infrastructure compliance indicators across 5 corridors.
* `processed_pwd_survey_n120.csv`: Summarized response metrics from N=120 PwDs questionnaire respondents.

## Code & Execution (`/scripts`)
The Python script `mcdm_accessibility_analysis.py` performs:
1. Integrated AHP–Entropy criteria weight calculations.
2. MCA-TOPSIS closeness coefficient (Cj+) evaluation.
3. Comparative MCDM algorithm execution (SAW, PROMETHEE II with Type V preference function, and VIKOR).
4. Rank concordance verification (rho = 1.00).

### Requirements
* Python 3.8+
* `numpy`, `pandas`, `scipy`

```bash
pip install numpy pandas scipy
python scripts/mcdm_accessibility_analysis.py
