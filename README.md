# Project Management Analytics Case

Which programs are at funding risk?

**Stakeholder:** Program Director

## Key Insights

- Three or more missed milestones precede at-risk funding reviews.
- Burn rate above 1.15x plan correlates with stakeholder escalation.
- Programs with 8+ stakeholders recover slower from milestone slips.

## Dataset

Primary file: `data/program_funding.csv`  
Target variable: `at_risk`

## Getting Started

```bash
pip install -r requirements.txt
jupyter notebook notebooks/01_exploration.ipynb
```


## Next Steps

**Done.** Class-weight tuning and SHAP explainability are implemented — see ### Implemented below.

---
*Analytics portfolio project — 2025-09*

<!-- build 6 -->

### Implemented

```bash
pip install -r requirements.txt
python src/train.py && python src/explain.py
```