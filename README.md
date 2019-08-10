# NISQ Implementations

A curated list of algorithm implementations on noisy, intermediate-scale quantum (NISQ) computers. Implemented algorithms are ordered chronologically and include architecture (e.g., superconducting), number of qubits, and references.

# Contributions

Please submit pull requests (or email rlarose (at) umich (dot) edu) with algorithm implementations not included below. Any and all corrections are welcome. References to open-access journals or the arXiv are preferred in all cases, if available. Markdown table generators such as [https://www.tablesgenerator.com/markdown_tables]() may be useful.

# Chronological ordering

| Year | Month     | Algorithm     | Problem Description                                          | Qubit type           | Computer                   | Number of Qubits | Reference                                                                                                                              |
|------|-----------|---------------|--------------------------------------------------------------|----------------------|----------------------------|------------------|----------------------------------------------------------------------------------------------------------------------------------------|
| 1997 | August    | Gate          | Implemented gates (XOR, Toffoli), prepared entangled state   | NMR                  | ----                       | 1-3              | https://arxiv.org/abs/quant-ph/9709001                                                                                                 |
| 1997 | October   | Gate          | Implemented gates (Rotation, CNOT), prepared entangled state | NMR                  | ----                       | 1-2              |                                                                                                                                        |
| 1997 | November  | Grover        | Executed Grover's algorithm on two qubits.                   | NMR                  | ----                       | 2                | [Paper](https://pdfs.semanticscholar.org/6c05/5053f4f1605fdc0bd474c7a350dcd01f627d.pdf)                                                |
| 1998 | January   | DJ            | Executed DJ algorithm on NMR quantum computer                | NMR                  | ----                       | 2                | https://arxiv.org/abs/quant-ph/9801027                                                                                                 |
| 1998 | February  | QEC           | Implemented 3-bit code for phase errors in liquid state NMR  | NMR                  |                            | 3                | https://arxiv.org/abs/quant-ph/9802018                                                                                                 |
| 1998 | August    | DJ            | Executed DJ algorithm on NMR quantum computer                | NMR                  | ----                       | 3                | https://arxiv.org/abs/quant-ph/9808039                                                                                                 |
| 2000 | March     | DJ            | Executed DJ algorithm on NMR quantum computer                | NMR                  | ----                       | 2-3              | https://journals.aps.org/pra/abstract/10.1103/PhysRevA.61.042306                                                                       |
| 2000 | June      | DJ            | Executed DJ algorithm on NMR quantum computer                | NMR                  | ----                       | ??               | https://aip.scitation.org/doi/10.1063/1.482015                                                                                         |
| 2000 | June      | DJ            | Executed DJ algorithm on NMR quantum computer                | NMR                  | ----                       | 4                | https://journals.aps.org/pra/abstract/10.1103/PhysRevA.62.012310                                                                       |
| 2001 | December  | Shor          | Factor 15                                                    | NMR                  |                            | 7                | https://arxiv.org/abs/quant-ph/0112176                                                                                                 |
| 2003 | January   | DJ/BV         | Implement DJ and BV on                                       | Linear optics        | ----                       | 3                | [Paper](https://pdfs.semanticscholar.org/0c3c/e11ac2926ad8974732958d98b10e9a7434ee.pdf)                                                |
| 2003 | February  | DJ            | Executed DJ on ion-trap quantum computer                     | Trapped ion (40Ca+)  | ----                       | 1                | [Paper](https://www.researchgate.net/publication/10964594_Implemention_of_the_Deutsch-Jozsa_algorithm_on_an_ion-trap_quantum_computer) |
| 2005 | September | DJ/Grover     | Implemented multiple algorithms on NMR quantum computer      | NMR                  | ----                       | ??               | https://arxiv.org/abs/quant-ph/0509046                                                                                                 |
| 2013 | April     | VQE           | Compute ground state energy of He-H+                         | Photonic             | ----                       | 2                | https://arxiv.org/abs/1304.3061                                                                                                        |
|      |           |               |                                                              |                      |                            |                  |                                                                                                                                        |
| 2015 | December  | VQE/QPE       | Compute energy surface of molecular Hydrogen                 | Superconducting      | ----                       | 2/3              | https://arxiv.org/abs/1512.06860                                                                                                       |
| 2016 | March     | DJ/BV/QFT     | Execute DJ, BV, and QFT algorithms                           | Trapped ion (171Yb+) | ----                       | 3-5              | https://arxiv.org/abs/1603.04512                                                                                                       |
| 2018 | February  | VQE/QSE       | Compute ground/excited states of H2                          | Superconducting      | ----                       | 2                | [PRX PDF](https://physics.aps.org/featured-article-pdf/10.1103/PhysRevX.8.011021)                                                      |
| 2018 | March     | S.O.          | Compute state overlap for one-qubit states                   | Superconducting      | IBMQX4, Rigetti 19Q        | 2                | https://arxiv.org/abs/1803.04114                                                                                                       |
| 2018 | April     | SVM           | Classify two-dimensional data                                | Superconducting      | ----                       | 2                | https://arxiv.org/abs/1804.11326                                                                                                       |
| 2018 | July      | QAQC          | Compile quantum algorithms                                   | Superconducting      | Rigetti 8Q-Agave, IBMQX1/2 | 2                | https://arxiv.org/abs/1807.00800                                                                                                       |
| 2018 | October   | VQSD          | Diagonalize a 2x2 matrix                                     | Superconducting      | Rigetti 8Q-Agave           | 1                | https://arxiv.org/abs/1810.10506                                                                                                       |
| 2019 | January   | QITE/QLanczos | Compute ground state energy of TFIM                          | Superconducting      | Rigetti Aspen-1            | 2                | https://arxiv.org/abs/1901.07653                                                                                                       |
| 2019 | March     | BV/HS         | Execute BV and HS algorithms                                 | Ion trap (171Yb+)    | ----                       | 11               | https://arxiv.org/abs/1905.09294                                                                                                       |
| 2019 | June      | Sim.          | Hamiltonian simulation for many-body dynamics                | Superconducting      | IBM 20Q                    | 6-10             | https://arxiv.org/abs/1906.06343                                                                                                       |                                                     |                                                |                                             |

## Algorithm keys (Alphabetical)

* BV: Bernstein-Vazirani.
* DJ: Deustch-Jozsa.
* HS: Hidden shift.
* QAQC: Quantum-assisted quantum compiling.
* QFT: Quantum Fourier Transform.
* QPE: Quantum phase estimation.
* QSE: Quantum subspace expansion.
* S.O.: State overlap.
* VQE: Variational quantum eigensolver.
* VQSD: Variational quantum state diagonalization.
