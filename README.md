# Generalized Sub Space Search VQE for Kth excited state energy

The goal of the project is to explore the ***Sub Space Search VQE Algorithm*** to calculate the Kth excited state energy of a given hamiltonian. There are three variants of SSVQE shown below:

* **Sub Space Search VQE:** The algorithm uses two step optimization process to calculate the Kth excited state energy.
* **Weighted Sub Space Search VQE to find energy of Kth excited state:** The algorithm uses one step optimization process to calculate the Kth excites state energy. 
* **Weighted Sub Space Search VQE to find energies upto K excited states:** The algorithm calculates all the excited state energies upto the Kth state in a single optimization process. The only drawback is the runtime due to the complexity of the cost function.

This project aim towards comparing the results of all three algorithms and how they perform on noiseless and noisy systems.

> **Note:** Current version of the project contains the implementation of the **Second** and **Third** algorithm from the above mentioned algorithms. We plan to implement the First before the final submission.

## Requirements
Before you start with [SSVQE.ipynb](https://github.com/Jay-Patel-257/Qhack-2022/blob/main/SSVQE.ipynb) make sure to install the below requirements.<br>
`!pip install pennylane`<br>
`!pip install pennylane-qchem`

## References
* https://arxiv.org/pdf/1810.09434.pdf
