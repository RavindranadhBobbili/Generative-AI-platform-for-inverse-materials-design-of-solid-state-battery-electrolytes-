# GenMatDesign-AI
Generative AI for Inverse Materials Design of Solid-State Battery Electrolytes

## Overview
GenMatDesign-AI is a deployable Flask-based inverse materials design platform that combines:

- Conditional Variational Autoencoder (CVAE) for generative candidate design
- Surrogate neural network for property prediction
- Uncertainty-aware screening using MC dropout
- Token-level explanation for generated electrolyte sequences
- Web dashboard and REST API deployment

Instead of testing a material and then measuring properties, this system accepts desired target properties and generates candidate electrolyte compositions likely to satisfy them.

## Domain
This prototype is focused on **solid-state battery electrolytes** represented as token sequences such as:

- `PEO-LiTFSI-SN-Al2O3`
- `PEGDA-LiFSI-EC-LLZO`

## Features
- Built-in internal electrolyte dataset
- No CSV upload required
- Train from internal library with one click
- Predict properties of a given electrolyte sequence
- Generate new candidates from desired target properties
- Rank candidates by closeness to target
- Estimate predictive uncertainty
- Token-importance style interpretation
- Web UI + REST API

## Tech stack
- Python
- Flask
- PyTorch
- NumPy
- Pandas
- Matplotlib

## Repository structure
```text
GenMatDesign-AI/
├── app.py
├── requirements.txt
├── Dockerfile
├── README.md
├── LICENSE
├── .gitignore
├── artifacts/
│   └── .gitkeep
├── static/
│   └── preview.png
└── docs/
    └── architecture.md
