# Responsibility Attribution Prediction

A computational framework for predicting responsibility attribution 
from regulatory violation text.

## Research Question
Can responsibility attribution (Firm / Individual / System) 
be predicted from violation text alone — and if so, 
what linguistic patterns drive each class?

## Key Findings
→ Individual-level attribution is most linguistically distinct 
  (AUC = 0.940, LOO-CV F1 = 0.85)
→ System-level attribution is most ambiguous 
  (AUC = 0.764), frequently confused with Firm
→ Model reassigns 49/160 FDA Firm-labeled violations to System, 
  suggesting regulatory documents mask infrastructure failures 
  under organizational accountability
→ Prediction confidence on FDA corpus is uniformly low (0.35–0.65), 
  indicating linguistic overlap between regulatory classes

## Methods
TF-IDF (unigram + bigram) · Logistic Regression / Random Forest / SVM  
Leave-One-Out CV · LIME interpretability · FDA Warning Letter corpus validation

## Dataset
- Annotated dataset (n=45, 3 classes balanced)
- FDA Warning Letter corpus (N=50, 160 violations, 2016–2025)

## Related Projects
- [Premature Convergence Detection](https://github.com/sorakim-lab/premature-convergence-detection)
- [Accountability Graph Extraction](https://github.com/sorakim-lab/accountability-graph-extraction)

## Reference
Kim, S. (2026). Anticipated Accountability Convergence. SSRN 6371980.
