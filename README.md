## Molecular Property Modeling with Machine Learning

Welcome! This repository brings together a suite of machine learning algorithms for molecular property prediction and optimization. Whether you’re a chemist exploring data-driven tools or a machine learning researcher diving into cheminformatics, you’ll find reproducible code, detailed explanations, and hands-on examples that bridge AI and molecular science.

We tackle two core problems:

1. Prediction — learning to estimate molecular properties like blood–brain barrier permeability from chemical structures.
2. Optimization — designing new molecules with improved properties (e.g., higher logP or drug-likeness) using generative and search-based techniques.

---

## Repository Overview

### 1. Molecular Property Prediction

This section focuses on supervised learning methods to classify or regress molecular properties from structural data, using the BBBP (Blood–Brain Barrier Penetration) dataset.

#### Techniques Implemented

| Model Type                  | Description                                                                                                                |
| --------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| Recurrent Neural Networks   | Uses GRUs to process SMILES strings as sequences. Captures long-range chemical dependencies.                               |
| Graph Neural Networks       | Treats molecules as graphs (atoms = nodes, bonds = edges). Includes GCNs, GATs, MPNNs with attention-based interpretation. |
| Random Forests              | Uses hand-crafted molecular descriptors (e.g., LogP, TPSA). Includes feature importance plots and model confidence tools.  |
| Feedforward Neural Networks | Uses descriptor vectors with dense neural networks. Supports SHAP analysis and model calibration visualizations.           |

#### Dataset Used

- `BBBP.csv`: A curated binary classification dataset indicating blood–brain barrier permeability. SMILES strings are used as input.

#### Tools & Libraries

- RDKit
- TensorFlow / Keras
- PyTorch Geometric
- Scikit-learn
- SHAP, matplotlib, seaborn

**Documentation:** [Molecular Property Prediction Docs](https://data-chemist-handbook.github.io/pages/Molecular_Property_Prediction/)

---

### 2. Molecular Property Optimization

This section showcases how machine learning can design molecules with desirable traits—such as increased lipophilicity (logP)—using intelligent search and generation methods.

#### Optimization Strategies

| Method                        | Description                                                                                                        |
| ----------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| Genetic Algorithms            | Evolves populations of molecules (SMILES strings) using mutation and crossover while preserving chemical validity. |
| Bayesian Optimization         | Uses Gaussian Process Regression (GPR) as a surrogate model with Expected Improvement to guide chemical search.    |
| Conditional Generative Models | Trains Conditional VAEs to generate novel molecules satisfying target property constraints. Uses PyTorch and ZINC. |

#### Goals

- Optimize logP or other scalar-valued molecular properties
- Ensure chemical validity of generated structures
- Compare evolutionary, probabilistic, and generative search paradigms

**Documentation:** [Molecular Property Optimization Docs](https://data-chemist-handbook.github.io/pages/Molecular_Property_Optimization/)

---

## Getting Started

You can run all models interactively in Google Colab or locally via Python 3.9+. Each subfolder includes:

- `notebooks/`: Annotated tutorials and visualizations
- `models/`: Architecture implementations
- `data/`: Input datasets or download links
- `requirements.txt`: Install dependencies using `pip install -r requirements.txt`

### Quick Start Example

```bash
git clone https://github.com/your-username/molecular-property-modeling.git
cd molecular-property-modeling/prediction
pip install -r requirements.txt
python run_rnn_bbbp.py
```

---

## Why This Matters

In cheminformatics and drug discovery, it’s crucial to both predict how molecules behave and generate new candidates with improved profiles. This repo equips you to:

- Learn from existing chemical structures
- Generate novel, property-optimized compounds
- Integrate AI into experimental and computational chemistry workflows

---

If this repo helps your research or learning, consider starring it or sharing with others in the community.

---

