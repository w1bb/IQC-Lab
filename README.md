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

## A quick history lesson

According to [JustPaste.it](https://justpaste.it/9trhs), Qiskit has a rich
history of development and evolution that can be traced back to 2017's IBM
first release. Back then, the simulator was nothing more than a Python library
based on the _matrix product state (MPS)_ and the
_time-evolving block decimation method (TEBD)_.

In 2018, IBM introduces noisy quantum circuits using the
_quantum process tomography (QPT)_ technique. This allowed for realistic
simulations that took into account the effect of noise and errors in the real
quantum hardware.

Once again, in 2019, IBM introduced a new feature, the Aer quantum simulator,
a high-performance program that can simulate large-scale quantum circuits with
millions of qubits and gates.

In recent years, that is in 2020, IBM made public Qiskit Runtime, which allows
users to run quantum circuits on real quantum hardware using IBM's API.

## Environment setup

While a detailed overview of the installation is provided by
[Qiskit themselves](https://qiskit.org/documentation/getting_started.html),
we've outlined the most important steps in this subsection. Please follow the
tutorial that is right for your platform.

### Windows

First, install [**Python 3**](https://www.python.org/downloads/) by clicking on
the yellow "Download Python 3.X.X" button and following the wizard's
instructions. Once that is done, you can check that both Python and its package
manager, **PiP**, were properly installed. To do this, open up a command prompt
and type:

```bash
python3 --version
pip3 --version
```

You should not get an error. If everything went alright, type in the same
command prompt the following:

```bash
pip3 install jupyter jupyterlab qiskit[visualization]
```

This command will automatically install everything we need in order to correctly
run **Qiskit** inside a **Jupyter lab** environment.

You can now move on to the next section.

### Linux

Install Python, PiP, Jupyter and VSCode. For **Ubuntu**, you can type in the
following in a terminal window:

```bash
sudo apt update
sudo apt install python3 python3-pip
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

To get started, you should run `jupyter-lab` inside a command line. In case
something goes wrong and an error pops up, you might need to log out and log
back in before continuing; on Linux, you can skip this step by simply running
`~/.local/bin/jupyter-lab` instead.

A browser should get launched alongside a locally hosted server. In the left
panel, please navigate to the folder in which you have downloaded/cloned this
repository. Now click on the `lab-QFT.ipynb` to load it and follow the
instructions provided in that notebook.

If, at any point, you get a little stuck, ask for help and/or take a look at the
proposed solution (see `lab-QFT-solution.ipynb`). Once you are done with that
notebook, you can move on to `lab-QPE.ipynb`.
