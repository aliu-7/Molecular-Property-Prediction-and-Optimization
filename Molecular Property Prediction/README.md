Molecular-Property-Prediction-Algorithms

This repository provides end-to-end implementations of machine learning models used to predict molecular properties directly from chemical structures. The models are evaluated using the BBBP (Blood–Brain Barrier Penetration) dataset, a key benchmark in pharmacokinetic modeling. Each approach is designed to handle a different molecular representation format—ranging from SMILES strings to graph-structured data and hand-crafted descriptors.

1. Recurrent Neural Networks (RNNs)

Leverages the sequential nature of SMILES strings to predict molecular properties using GRU-based RNNs. Each molecule is tokenized at the character level and processed one step at a time to capture long-range dependencies and syntactic structure.
	•	Application: Classifying molecules as BBB-permeable vs. impermeable.
	•	Dataset: BBBP (binary labels, SMILES input).
	•	Tools: TensorFlow, Keras.
	•	Bonus: Includes hidden-state visualizations and embedding comparison (one-hot vs. learnable).

2. Graph Neural Networks (GNNs)

Models molecules as graphs, where atoms are nodes and bonds are edges. The GNN architecture learns to propagate chemical signals through message passing, enabling the capture of topological and electronic structure directly.
	•	Application: BBBP classification using molecular graph input.
	•	Models: GCN, GAT, MPNN (PyTorch Geometric).
	•	Tools: RDKit, PyG.
	•	Bonus: Includes interpretable GAT attention scores and graph construction tutorials.

3. Random Forests on Molecular Descriptors

Applies ensemble decision tree methods to classify molecules using RDKit-computed physicochemical descriptors (e.g., LogP, TPSA, rotatable bonds). Ideal for interpretable baseline models on small- to mid-sized datasets.
	•	Application: Descriptor-based BBBP classification.
	•	Tools: Scikit-learn, RDKit.
	•	Bonus: Includes descriptor importance plots and model confidence analysis.

4. Feedforward Neural Networks (FNNs)

Uses fully connected neural networks to model relationships between molecular descriptors and target properties. A modern alternative to random forests when working with tabular chemical data.
	•	Application: Binary classification using standardized descriptor vectors.
	•	Tools: TensorFlow/Keras, RDKit.
	•	Bonus: Includes permutation importance, SHAP analysis, and calibration visualizations.

⸻

Documentation & Code Notebooks
All code is runnable in Google Colab and available in the corresponding subfolders. Each chapter includes step-by-step Jupyter notebooks and visualizations.


Companion Material:
Extended textbook-style explanations and interactive notebooks are available at: https://data-chemist-handbook.github.io/pages/Molecular_Property_Prediction/