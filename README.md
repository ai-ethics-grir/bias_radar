
⚠️ **Disclaimer**  
This repository contains demonstration code and synthetic data for AI Ethics PoCs.
It is not production-ready. Unauthorized commercial use is prohibited.

# Bias Radar for AML/Credit

**Author:** Grimaldi Roberto | AI Ethics  
Monitors and mitigates unfairness in AML/credit models with alerting and reports.

## Setup
```bash
pip install -r requirements.txt
streamlit run app.py
```

## Logical Steps
1. Choose fairness definitions (EO, DP, Equalized Odds).
2. Identify sensitive attributes; ensure sample sufficiency.
3. Train baseline and compute metrics with confidence intervals.
4. Threshold sweep to map performance–fairness trade-offs.
5. Apply mitigations (reweighing, post-processing) and re-evaluate.
6. Real-time alerts for metric breaches.
7. Monthly/quarterly re-calibration cadence.
8. Publish fairness report for each release.

## KPIs
- Business: Customer complaints ↓ ≥20%.
- Ethics: Equal Opportunity Difference ≤ 5%.
- Compliance: FINMA non-discrimination adherence; audit trail.

## Files
- `app.py` — Streamlit dashboard.
- `reports/fairness_report.md`, `reports/model_card.md`
- `assets/cover.png` — cover image placeholder.
