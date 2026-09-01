# Fraud Detection — Engineering & Business Investigation

> **An engineering and business investigation into machine learning for fraud detection.**

## Overview

Fraud detection is not simply a problem of classifying transactions as fraudulent or legitimate.

It is a problem in which **statistical modeling, decision-making and business consequences intersect under severe class imbalance**.

This project investigates that problem through a sequence of empirical studies using machine learning and a public fraud-detection dataset.

The purpose is not to provide a generic implementation or a prescriptive methodology.

It is to examine the problem from an engineering perspective and document selected findings that emerge from the investigation.

---

## The Problem

Fraud detection involves asymmetric consequences.

Failure to identify fraudulent activity can result in financial and operational losses.

Incorrectly identifying legitimate activity can generate customer friction, operational workload and other business consequences.

This makes conventional classification accuracy an inadequate standalone measure of system usefulness.

The relevant challenge is therefore not simply:

> **Can a model classify transactions accurately?**

but rather:

> **Can machine learning provide useful information for making better decisions under the constraints of a real-world fraud-detection problem?**

---

## Why Accuracy Is Not Enough

Fraud represents a very small proportion of transactions in the dataset used in this investigation.

Consequently, a classifier can achieve approximately **99.83% accuracy while detecting no fraudulent transactions**.

The result is statistically plausible but operationally ineffective.

This provides the initial reference point for the investigation:

> **A strong aggregate metric does not necessarily imply useful performance on the problem that matters.**

The observation motivates the subsequent investigation into alternative evaluation perspectives.

---

## Engineering Perspective

The project approaches fraud detection as an engineering problem rather than as an isolated model-training exercise.

The investigation considers the relationship between:

```text
Data
  ↓
Model
  ↓
Prediction
  ↓
Evaluation
  ↓
Decision
  ↓
Operational Consequence
```

The individual studies examine selected aspects of this relationship.

Implementation details, experimental procedures and decision mechanisms are intentionally limited to the material necessary to communicate the published findings.

---

## Research Cases

The investigation is organized as a sequence of research cases.

### Research Case #001

The first study establishes the problem through a deliberately simple reference and examines the limitations of conventional evaluation under severe class imbalance.

The study demonstrates why the apparent performance of a classifier must be interpreted in the context of the underlying problem.

### Research Case #002

The second study extends the investigation beyond the initial model-performance perspective and examines a subsequent engineering question arising from the evidence.

The complete experimental methodology and implementation are presented selectively rather than as a prescriptive solution.

Additional research cases may follow as new questions emerge from the investigation.

---

## Selected Evidence

The initial investigation established a fundamental observation:

|Reference|Accuracy|Fraud Recall|
|---|--:|--:|
|Majority-class baseline|≈99.83%|0%|

This result is intentionally simple.

Its significance lies not in the baseline itself, but in what it demonstrates about evaluating machine learning systems under severe class imbalance.

Further findings are documented in the corresponding research publications.

---

## What This Project Demonstrates

The project focuses on demonstrating capabilities in:

- problem formulation;
    
- experimental reasoning;
    
- imbalanced classification;
    
- model evaluation;
    
- statistical interpretation;
    
- engineering trade-offs;
    
- decision-oriented machine learning;
    
- connecting technical evidence with business context.
    

The emphasis is on **how an engineering problem is reasoned about**, rather than on providing a turnkey implementation.

---

## What This Project Is Not

This project is not:

- a production fraud-detection system;
    
- a generic machine learning tutorial;
    
- a step-by-step implementation guide;
    
- a collection of isolated algorithms;
    
- a benchmark claiming universal model superiority;
    
- a complete blueprint for reproducing a production fraud-detection solution.
    

The repository deliberately separates **demonstration of expertise** from **transfer of an entire implementation methodology**.

---

## Data

The experiments use the public credit card fraud dataset commonly distributed as `creditcard.csv`.

The dataset contains anonymized transaction features and a binary target representing legitimate and fraudulent transactions.

It provides a controlled environment for investigating machine learning techniques and decision-making under severe class imbalance.

The results should not be interpreted as evidence of production performance in a financial institution.

---

## Limitations

A public benchmark cannot reproduce the full complexity of a production fraud-detection environment.

Real-world systems may involve factors that are outside the scope of the experimental environment and should be considered independently when moving from research to production.

---

## Publications

The investigation is documented through a sequence of technical publications.

- **Research Case #001** — establishes the initial problem and baseline evidence.
    
- **Research Case #002** — investigates a subsequent engineering question arising from the first study.
    

The publications intentionally focus on **findings, reasoning and evidence**, rather than presenting a complete recipe for solving fraud detection.

---

## Repository Structure

```text
fraud-detection/
├── README.md
└── article/
    ├── figures/
    │   ├── figure_01_precision_recall_threshold.png
    │   └── ...
    ├── Establishing a Meaningful Baseline.md
    ├── ranslating Fraud Risk into Operational Actions.md
    └── ...
```

The repository will evolve as additional research cases are published.

---

## Research Philosophy

The investigation follows a simple principle:

> **Technical complexity should be supported by evidence.**

Models, metrics and engineering decisions are therefore treated as components of an investigation rather than as objectives in themselves.

The work emphasizes:

```text
Problem
   ↓
Evidence
   ↓
Reasoning
   ↓
Engineering Decision
```

The specific mechanisms used to obtain individual findings are intentionally not presented as a turnkey methodology.

---

## Business Perspective

The ultimate concern is not the isolated performance of a machine learning model.

It is whether the information produced by the model can contribute to a decision that is technically defensible and relevant to the business context.

The investigation therefore considers machine learning as one component of a broader decision system.

No claim is made that the experiments establish a universally optimal business policy.

---

## Author

**Francisco Ortiz**

Engineering · Software Architecture · Machine Learning · Artificial Intelligence

---

## Disclaimer

This repository represents an experimental investigation using a public dataset.

It should not be interpreted as financial, fraud-prevention, regulatory or production-system advice.
