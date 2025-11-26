Part 2 — Case Study Analysis (40%)

Case 1: Biased Hiring Tool (Amazon recruiting example)

Scenario recap: An automated recruiting model penalized female candidates because historical hiring data reflected male dominance in certain roles.

a) Source(s) of bias
- Historical training data skew: The model learned from past hiring decisions that favored men.
- Feature leakage and proxies: Certain features (e.g., attendance at male-dominated schools, specific keywords) acted as proxies for gender.
- Objective mis-specification: Optimizing purely for historical hire likelihood perpetuates past discrimination.

b) Three fixes to make the tool fairer
1. Data rebalancing & augmentation: Gather more representative positive examples for underrepresented genders, or use reweighting to reduce bias in training set.
2. Feature review & de-biasing pipelines: Remove or transform proxy features correlated with sensitive attributes; use adversarial debiasing to reduce sensitive-attribute information in representations.
3. Post-processing fairness constraints: Apply fairness-aware selection (e.g., calibrated equalized odds post-processing) and include human-in-the-loop review for borderline candidates.

c) Metrics to evaluate fairness post-correction
- Disparate impact ratio (selection rate ratio between protected and privileged groups).
- Equal opportunity difference (difference in true positive rates across groups).
- False negative rate gap (important for hiring: ensure qualified candidates aren't wrongly rejected).
- Calibration within groups (ensure predicted scores have same meaning across groups).

Case 2: Facial Recognition in Policing

Scenario recap: A facial recognition system misidentifies minorities at higher rates than others.

a) Ethical risks
- Wrongful arrests and criminal justice harm: Higher false positive rates for minorities can lead to unjust detentions.
- Privacy violations and chilling effects: Widespread deployment increases surveillance, disproportionately impacting vulnerable communities.
- Reinforcement of systemic bias: Aggregate harms exacerbate distrust between communities and institutions.
- Due process and accountability gaps: Lack of human oversight or opaque use hinders redress for affected individuals.

b) Recommended policies for responsible deployment
- Prohibit use for sole evidence: Disallow automated matches from being the only basis for arrest; require additional independent corroboration.
- Strict accuracy & bias thresholds: Require independent audits demonstrating acceptable error rates across demographic groups before deployment.
- Limited scope and logging: Narrow use cases (e.g., investigations with probable cause), retention limits, and full audit logs for accountability.
- Community engagement & oversight: Public reporting, external audits, and community consent where deployment affects specific populations.
