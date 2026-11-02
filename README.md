# speed_dating_attraction_analysis
Speed Dating Analytics : Attraction, Behavioral Insights & ML

# Speed Dating — What Drives Attraction?

**Data Analytics | Statistical Inference | Logistic Regression | Python**

**Author:** Schuyler Gilmer-Gonçalves  
**Project:** RNCP 35288, Bloc 2 (2026)

> Academic case study inspired by dating-platform product analytics. Dataset: Columbia Business School Speed Dating Experiment (2002–2004). This project is not affiliated with Tinder and does not use Tinder user data.

---

## English

### Project Overview

What drives romantic attraction? Do people choose partners based on their stated preferences, or do their decisions reveal different priorities?

This project analyzes historical speed-dating data using exploratory data analysis, hypothesis testing and logistic regression.

### Dataset

- **8,378** individual evaluations
- **4,184** unique encounters
- **551** participants
- **195** original variables
- **16.5%** reciprocal match rate

**Source:** [Columbia Speed Dating Experiment — Kaggle](https://www.kaggle.com/annavictoria/speed-dating-experiment)

Download the dataset, rename it `speed_dating.csv`, and place it in `data/raw/` to run the notebook.

### Methodology

1. Data quality checks and preprocessing
2. Chi-square tests and Welch t-tests
3. Cohen's d effect sizes and correlation analysis
4. Multivariate logistic regression
5. Comparison between stated preferences and observed decisions
6. ROC-AUC model evaluation

### Key Findings

**1. Selectivity differs between groups**

In this sample, women accepted 36.5% of dates, compared with 47.4% for men.

**2. Perceived attractiveness is strongly associated with positive decisions**

A one-standard-deviation increase in perceived attractiveness was associated with approximately 2.9 times higher odds of saying yes, conditional on the other modeled ratings.

**3. Stated preferences have limited predictive power**

| Model | Test ROC-AUC |
|---|---:|
| Stated preferences | 0.51 |
| Post-interaction ratings | 0.81 |
| Combined | 0.82 |

The models predict an individual's yes/no decision, not a reciprocal match.

**4. Self-perception differs from external evaluations**

Participants rated themselves approximately 0.8–1.3 points higher than the average ratings they received across five attributes.

**5. Perceived similarity matters more than measured similarity**

Perceived shared interests were positively associated with the yes/no decision (r ≈ 0.40), while the measured interest-similarity indicator showed little correlation (r ≈ 0.02).

### Business Implications

The results suggest exploring behavioral signals, reciprocal-match prioritization and perceived compatibility in dating-platform product design.

These are hypotheses for product experimentation, not proven causal effects.

### Limitations

The data were collected in 2002–2004 during face-to-face speed-dating events, not on a modern dating app. Observational associations do not establish causality. The random row-based train/test split may also overestimate generalization to unseen participants.

### Project Files

- [Full Jupyter Notebook](notebooks/speed_dating_analysis.ipynb)
- [Executive Presentation](presentation/speed_dating_findings.pdf)

---

## Français

### Présentation

Quels facteurs influencent l'attirance et la décision de revoir une personne ? Les préférences déclarées prédisent-elles réellement les choix ?

Ce projet analyse les données d'expériences de speed dating de Columbia (2002–2004), en combinant statistiques descriptives, tests d'hypothèses et régression logistique.

### Données et méthodologie

L'étude porte sur 8 378 évaluations individuelles, correspondant à 4 184 rencontres uniques et 551 participants.

Les analyses comprennent la qualité des données, les tests du khi-deux et de Welch, les tailles d'effet, les corrélations et trois modèles de régression logistique.

### Principaux résultats

**1. Sélectivité :** 36,5 % de décisions positives chez les femmes contre 47,4 % chez les hommes dans cet échantillon.

**2. Attractivité :** l'attractivité perçue est l'un des facteurs les plus fortement associés à une réponse positive (odds ratio ≈ 2,9 pour +1 écart-type).

**3. Déclaré versus observé :** les préférences déclarées produisent une AUC de 0,51, contre 0,81 pour les évaluations après interaction et 0,82 pour le modèle combiné.

**4. Perception de soi :** les participants s'autoévaluent généralement entre 0,8 et 1,3 point au-dessus des évaluations reçues.

**5. Similarité :** la similarité perçue est davantage associée à une réponse positive que la similarité mesurée des centres d'intérêt.

### Applications métier

Le projet propose d'explorer des approches fondées sur les comportements observés, la réciprocité et la perception de compatibilité.

Ces recommandations nécessiteraient des expérimentations avant tout déploiement produit.

### Limites

L'échantillon historique n'est pas représentatif des utilisateurs actuels de Tinder. Les corrélations ne prouvent pas de relation causale, et la validation prédictive pourrait être renforcée par une séparation des participants entre entraînement et test.

### Livrables

- [Notebook Python](notebooks/speed_dating_analysis.ipynb)
- [Présentation du projet](presentation/speed_dating_findings.pdf)



**Academic Data Analytics Project — 2026**