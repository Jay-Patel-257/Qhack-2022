# Weighted Subspace Search VQE to find Kth Excited state energies

Generally, The variational quantum eigensolver (VQE) is used for finding the ground state energy for a given hamiltonian. To find the kth excited state energy of for the hamiltonian we would need to run the VQE optimization process for atleast k+1 time. Not to mention each time we need to calculate the hamiltonian again taking into account the state of the previous iteration. Even after that the accuracy decreases as value of k increases.

This is where the idea of ***Subspace Search VQE (SSVQE)*** comes in. The algorithm is used to find kth excited state energy of a hamiltonian in just two subsequent optimization processes. The original research about the development of SSVQE is given in this [paper](https://arxiv.org/pdf/1810.09434.pdf). But, can we do better? Yes, the research shows that using the weights as hyperparameters we can find the kth excited state energy in just single optimization process. This is a more generalised version of SSVQE namely, Weighted SSVQE and it will be the center of our focus in this project. There are two variants of this algorithm:

1) Weighted SSVQE to find kth excited state energy.

2) Weighted SSVQE to find all energies upto kth excited state.

We simulated three different Hamiltonians of molecules like H2, LiH and CH3F using three algorithms that we implemented in this project. Yes, the third one is surprise for you so for more detalied info go check out [SSVQE.ipynb](./SSVQE.ipynb)

## Results of Simulation:
> The graphs are drawn for Iteration vs Energy.
### H2:
![H2_1](./Img/H2_1.png)![H2_2](./Img/H2_2.png)![H2_3](./Img/H2_3.png)
### LiH:
![LiH_1](./Img/LiH_1.png)![LiH_2](./Img/LiH_2.png)![LiH_2](./Img/LiH_3.png)
### CH3F:
![CH3F_1](./Img/CH3F_1.png)![CH3F_2](./Img/CH3F_2.png)![CH3F_2](./Img/CH3F_3.png)

## Requirements
Before you start with [SSVQE.ipynb](https://github.com/Jay-Patel-257/Qhack-2022/blob/main/SSVQE.ipynb) make sure to install the below requirements.<br>
`!pip install pennylane`<br>
`!pip install pennylane-qchem`

## Presentation:
[Link](https://docs.google.com/presentation/d/1P1tNo31xcmKQOwSVYmKvNdP2JYbssHYmoEam_dHvJ9U/edit?usp=sharing)

## Prepared by
**Jay Patel ([@Jay-Patel-257](https://github.com/Jay-Patel-257))**<br>
**Siddharth Patel ([@Siddharth1India](https://github.com/Siddharth1India))**<br>
**Amit Hirpara ([@HirparaAmit](https://github.com/HirparaAmit))**

## References
* https://arxiv.org/pdf/1810.09434.pdf
* https://pubchem.ncbi.nlm.nih.gov/1
> [SSVQE.ipynb](./SSVQE.ipynb) has been approved for pennylane community tutorials and can be found at [Pennylane Community Tutorials](https://pennylane.ai/qml/demos_community.html).
