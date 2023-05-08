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
repository. Now click on the `lab.ipynb` and follow the instructions provided in
that notebook.