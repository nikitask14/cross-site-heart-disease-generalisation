# Cross-Site Heart Disease Generalisation

A research-oriented machine learning capstone investigating model behaviour across multiple data-collection sites using the UCI Heart Disease dataset.

## Project Purpose

This project is designed to study **multi-site heterogeneity and cross-site generalisation under centralized learning**.

The broad question is:

> Can a model trained using centrally pooled multi-site data perform consistently across the different sites represented in the dataset?

The exact research question and experimental design will be refined after understanding the dataset.

## Dataset

The project uses the UCI Heart Disease collection, which contains data associated with four sources:

* Cleveland
* Hungary
* Switzerland
* VA Long Beach

The project will first examine these sites separately before making decisions about pooling, modelling, and evaluation.

## Target

The original num target is converted into a binary classification problem:

* 0 → heart disease absent
* 1–4 → heart disease present

The original num column is retained for traceability.

## Experimental Design

Each site is split separately into:

* 60% training
* 20% validation
* 20% test

The split is stratified using the binary target.

Corresponding site-specific subsets are then pooled to create centralized training, validation, and test sets, while the individual site test sets are retained for cross-site evaluation.

Current pooled split sizes:

Train: 550
Validation: 185
Test: 185

**Stage 1 — Dataset understanding**

Current tasks include:

* understanding the raw data files,
* identifying the variables using the official data documentation,
* examining site sizes,
* checking data types and missing values,
* understanding the recorded outcome,
* investigating differences between sites.

No final modelling or evaluation decisions have yet been made.

## Planned Research Workflow

Dataset understanding
→ target understanding
→ ML problem definition
→ research question
→ experimental design
→ evaluation strategy
→ preprocessing
→ classical baseline
→ neural-network baseline
→ controlled experiments
→ reproducibility checks
→ interpretation
→ limitations
→ next research question

## Current Stage

Preprocessing

## Scope

This is a research-training project.

The UCI Heart Disease collection is a historical dataset. Results will therefore be interpreted only within this dataset and experimental setting and will not be presented as contemporary clinical conclusions.

This project uses **centralized learning**. Federated learning and FedAvg will be investigated separately after this capstone.

## Status

Work in progress.
