Meta-Learning: Rapid Adaptation via MAML, Reptile, and Prototypical Networks

This repository contains the code, experiments, and tutorial for a meta-learning project comparing three major algorithms: Model-Agnostic Meta-Learning (MAML), Reptile, and Prototypical Networks. The goal is to demonstrate how these methods enable rapid adaptation in few-shot classification tasks and to evaluate their behaviour across 1–5 gradient steps.

Repository Structure
├── notebooks/
│   └── machine code.ipynb      # Jupyter notebook with full code
├── figures/
│   ├── meta_training_curves.png
│   ├── adaptation_curves.png
│   ├── decision_boundary_maml_0.png
│   ├── decision_boundary_maml_5.png
│   └── decision_boundary_random_0.png
├── tutorial.pdf                              # Final report (<2000 words)
├── src/
│   └── models.py                              # Optional modular code
├── LICENSE                                    # MIT License
└── README.md

How to Run the Code

Install dependencies:

pip install torch matplotlib numpy scikit-learn


Open the Jupyter notebook:

jupyter notebook notebooks/machine code.ipynb


Run all cells to:

Train MAML

Evaluate Reptile and Prototypical Networks

Generate adaptation curves

Produce decision boundary visualisations

Export figures for the report

All results shown in the tutorial can be fully reproduced from this notebook.

Dataset Description

Tasks are synthetically generated 3-way, 5-shot Gaussian classification problems. Each classification task uses:

Support set: 5 samples per class

Query set: 15 samples per class

Input space: 2-dimensional vectors

This structure enables visual interpretation of meta-learning behaviour while keeping computation fast.

Accessibility Notes

All plots use colour-blind-friendly palettes.

Figures include clear axis labels and high-contrast backgrounds.

Decision boundaries use shape + position cues, not colour alone.

The tutorial PDF uses descriptive alt text for every figure.

License

This project is released under the MIT License. See the LICENSE file for details.
