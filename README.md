# Aligning (Medical) LLMs for (Counterfactual) Fairness

Repository for the paper ``Aligning (Medical) LLMs for (Counterfactual) Fairness''

Our repository is divided into two parts: eval, and mitigation.

![framework-1](https://github.com/user-attachments/assets/159b5f11-ce8a-41a5-8924-6eec675f8335)
The eval folder contains the code required to run the evaluation framework for each dataset presented in the paper.

![diagram-1](https://github.com/user-attachments/assets/1626ebf7-e5be-4d29-ab33-190a069003ba)
The mitigation folder contains the code to align the LLMs for counterfactual fairness. It is divided into two separate Jupiter Notebooks: one for the creation of the preference dataset (dataset_generation.ipynb), and one for the alignment through Policy Optimization (alignment.ipynb).
Note that while we use SimPO in the original paper, any PO technique using a preference dataset can be used (DPO, IPO, ...). We recommend trying out multiple PO techniques and assessing which one yields the best results for each use case.
