# Parameterized Hamiltonian Fitting for Trivalent Lanthanide Ions

This repository contains Python code and scripts, designed to perform a parameterized fitting of the Hamiltonian for the trivalent lanthanide ions, by utilizing advanced optimization techniques. The project leverages two primary approaches: hyperparameter optimization using Optuna and PyTorch.

## Repository Contents

### Main Files

1. **`Optuna-lanthanide-fitting.ipynb`**
   - Utilizes [Optuna](https://optuna.org/), a hyperparameter optimization framework, to perform a broad search over parameter ranges.
   - Aims to match the Hamiltonian's eigenvalues with a given set of energy levels by exploring a wide parameter space efficiently.
   - Ideal for initial, exploratory optimization to determine rough parameter bounds.

2. **`PyTorch-lanthanide-fitting.ipynb`**
   - Utilizes [PyTorch](https://pytorch.org/), for gradient-based optimization, enabling fine-tuning of parameters with precision.
   - Matches the Hamiltonian's eigenvalues with a given set of energy levels using iterative refinement.
   - Best suited for detailed, localized parameter optimization after establishing a suitable range.

---

## Getting Started

### Prerequisites

Ensure you have the following dependencies installed:

- Python 3.8+
- Jupyter Notebook
- Required Python packages:
  - `torch`
  - `optuna`
  - `pandas`
  - `os`
  - `time`

## Usage

### Running the Optuna Fitting Script

1. Open `Optuna-lanthanide-fitting.ipynb` in your preferred Python notebook editor (e.g., Jupyter Notebook, VS Code, or PyCharm).
2. Follow the steps outlined in the notebook to:
   - Convert the symbolic Hamiltonian (exported from Mathematica code, see [qLanth](https://github.com/zia-lab/qlanth), into python language).
   - Define target eigenvalues for the Hamiltonian.
   - Specify the fitting parameters and their respective ranges.
   - Perform hyperparameter optimization using the Optuna framework.
   - Save detailed results from the optimization, including the best-fit parameters and the iteration process.

### Running the PyTorch Fitting Script

1. Open `PyTorch-lanthanide-fitting.ipynb` in your preferred Python notebook editor (e.g., Jupyter Notebook, VS Code, or PyCharm).
2. Follow the steps outlined in the notebook to:
   - Convert the symbolic Hamiltonian (exported from Mathematica code, see [qLanth](https://github.com/zia-lab/qlanth), into python language).
   - Define target eigenvalues for the Hamiltonian.
   - Specify the fitting parameters and their initial values.
   - Perform hyperparameter optimization using the Python framework.
   - Compute the uncertainties of the optimized parameters.
   - Save detailed results from the optimization, including the best-fit parameters and the iteration process.


---

## Acknowledgments

- [Optuna](https://optuna.org/): "An open source hyperparameter optimization framework to automate hyperparameter search."
- [PyTorch](https://pytorch.org/): "A neutral home for the deep learning community to collaborate on the open source PyTorch framework and ecosystem."

