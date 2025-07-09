Recurrent Neural Networks (RNNs) are a type of deep learning architecture designed to process sequential data—making them especially powerful for tasks involving temporal order or structural dependencies. In chemistry, this makes RNNs a natural fit for working with SMILES strings, a linear representation of molecules that encodes structural information using a sequence of characters.

Unlike traditional feedforward neural networks, which treat each input independently, RNNs maintain a hidden state that carries contextual information from one step of the sequence to the next. This allows them to capture dependencies across a molecular structure that are expressed sequentially, such as ring closures or branches that appear far apart in the SMILES string but are chemically related.

