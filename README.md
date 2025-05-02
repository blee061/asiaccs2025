# ACM AsiaCCS'25 POSTER: Stealthy SWAP-Based Side-Channel Attack on Multi-Tenant Quantum Cloud Systems

* Important Note: From [1 July 2025](https://docs.quantum.ibm.com/migration-guides/classic-iqp-to-cloud-iqp), the IBM Quantum Platform Classic will no longer be available. As a result, the code in the Python notebooks may not function as expected. Furthermore, with the release of [Qiskit V2.0](https://www.ibm.com/quantum/blog/qiskit-2-0-release-summary), "_this major version does break compatibility with previous versions of Qiskit_" (quoted from the [V2.0 docs](https://docs.quantum.ibm.com/migration-guides/qiskit-2.0)), which may require refactoring of the code for it to run properly.

# Repository Contents
This GitHub Repository contains the following resources which are included in the ACM ASIACCS 2025 Conference Paper titled `POSTER: Stealthy SWAP-Based Side-Channel Attack on Multi-Tenant Quantum Cloud Systems`:
1. `README.md` (This document)
2. `requirements.txt`
3. `Experiment 1 Active SWAP Attack.ipynb` Python Notebook
4. `Experiment 2 Passive SWAP Attack.ipynb` Python Notebook
5. `.gitignore`

# requirements.txt
A `requirements.txt` file is provided in this repository to ensure that all necessary dependencies are installed for running the Python notebooks without issues. Users may install the required packages using one of the following methods:

1. Termainal Installation
    1. Open terminal
    2. Paste `pip3 install -r requirements.txt` into terminal
    3. Enter to run
2. VS Code venv
    1. Open Python notebook
    2. Select kernel
    3. Select `Python Environments...`
    4. Select `Create Python Environment`
    5. Select `Venv`
    6. Select Python Interpreter
    7. Tick the checkbox for `requirements.txt` and click `OK`


# Missing Graphviz Library Error
The `plot_circuit_layout` function from `qiskit.visualization` requires the `Graphviz` library, which is not included in the pip installation process. If `Graphviz` is not installed, you may encounter the following error when running the `plot_circuit_layout` function:

> MissingOptionalLibraryError: "The 'Graphviz' library is required to use 'plot_coupling_map'.  To install, follow the instructions at https://graphviz.org/download/. Qiskit needs the Graphviz binaries, which the 'graphviz' package on pip does not install. You must install the actual Graphviz software."

For detailed installation instructions, users may visit the [Graphviz Webiste](https://graphviz.org/download/). Alternatively, users may also use one of the following installation commands, depending on the users' operating system:

## Mac
- Homebrew

`brew install graphviz`

- MacPorts

`sudo port install graphviz`

## Windows
- Chocolatey packages
  
`choco install graphviz`
- Windows Package Manager
  
`winget install graphviz`

## Linux
- Debian, Ubuntu
  
`sudo apt install graphviz`
- Fedora project, Rocky Linux, Redhat Enterprise Linux, or CentOS
  
`sudo dnf install graphviz`


