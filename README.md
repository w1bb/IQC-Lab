# IQC Lab - Qiskit, QFT, QPE and beyond!

The following repository is intended to store all the materials required to
fully implement the QFT (Quantum Fourier Transform) and the QPE (Quantum Phase
Estimation) algorithms.

Our simulator of choice is [**Qiskit**](https://qiskit.org/), since it provides
a great API and easy-to-use features.

## Authors

This lecture was kindly brought to you by:

- Cătălin-Alexandru RÎPANU ([@CatalinACS](https://github.com/CatalinACS));
- Valentin-Ioan VINTILĂ ([@w1bb](https://github.com/w1bb)).

All the resources were created entirely by us or were properly credited in the subsection below.

## Environment setup

While a detailed overview of the installation is provided by
[Qiskit themselves](https://qiskit.org/documentation/getting_started.html),
we've outlined the most important steps in this subsection. Please follow the
tutorial that is right for your platform.

### Windows

TODO?

### Linux

Install Python, PiP, Jupyter and VSCode. For **Ubuntu**, you can type in the
following in a terminal window:

```bash
sudo apt update
sudo apt install python3 python-pip
pip install jupyter jupyterlab qiskit[visualization]
```

Alternatively, **Arch** provides a different method:

```bash
sudo pacman -Syu
sudo pacman -S python python-pip
pip install jupyter jupyterlab qiskit[visualization]
```

If you are a ZSH user, you should place `qiskit[visualization]` in single
quotes, as in `pip install jupyter jupyterlab 'qiskit[visualization]'`.

## Running the lab

In order to get started, you should start `jupyter-lab` and open the `lab.ipynb`
file. Then, follow the instructions provided in the said document.

_Note:_ On Linux, running the `jupyter-lab` without logging off can only be
performed by running `~/.local/bin/jupyter-lab` from a terminal window.
