# Generelized Sub Space Search VQE for Kth excited state energy

The goal of the project is to explore the <b><i>Sub Space Search VQE Algorithm</i></b> to calculate the Kth excited state energy of a given hamiltonian. There are three variants of SSVQE shown below:

* <b>Sub Space Search VQE:</b> The algorithm uses two step optimization process to calculate the Kth excited state energy.
* <b>Weighted Sub Space Search VQE to find energy of Kth excited state:</b> The algorithm uses one step optimization process to calculate the Kth excites state energy. 
* <b>Weighted Sub Space Search VQE to find energies upto K excited states:</b> The algorithm calculates all the excited state energies upto the Kth state in a single optimization process. The only drawback is the runtime due to the complexity of the cost function.

This project aim towards comparing the results of all three algorithms and how they perform on noiseless and noisy systems.

> <b>Note:</b> Current version of the project contains the implementation of the second algorithm from the above mentioned algorithms. We plan to implement the rest in the final submission.

## Requirements
`!pip install pennylane`<br>
`!pip install pennylane-qchem`

## References
* https://arxiv.org/pdf/1810.09434.pdf
