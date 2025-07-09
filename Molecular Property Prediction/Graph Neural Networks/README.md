In cheminformatics, molecules are often represented in ways that strip away structural context—such as SMILES strings (linearized text) or tabular descriptors (e.g., LogP, molecular weight). While these formats are convenient for storage or computation, they lose the graph-based nature of chemical structure, where atoms are nodes and bonds are edges.

Graph Neural Networks (GNNs) are designed to work directly with this native molecular form. Rather than relying on handcrafted features or linearized input, GNNs learn directly from molecular graphs, capturing both local atomic environments and global topological patterns. This enables them to model nuanced chemical behavior—like electron delocalization, steric hindrance, or intramolecular interactions—that traditional models may overlook.

From predicting toxicity and solubility to quantum properties and biological activity, GNNs have become a cornerstone of modern molecular machine learning. They offer a powerful and general-purpose framework that reflects how chemists naturally think: in terms of atoms and their connections.

In this chapter, we’ll walk through:

- How molecules are converted into graphs for computation
- The concept of message passing—the core engine of a GNN
- Variants of GNN architectures commonly used in chemistry
- A full classification example using PyTorch Geometric (PyG)
- Practical considerations, limitations, and tuning strategies

GNNs are not just another model type—they represent a shift toward structure-aware learning, and mastering them opens the door to high-performance property prediction across drug discovery, materials science, and beyond.