# Unofficial-HTWG-LaTeX-Template

📄 This repository is intended as an unofficial LaTeX Template for documentations at the <br>
🗺️ University of Applied Sciences (HTWG) Konstanz.

🧭 The template aims to create latex documentation within VS code and export it to a pdf document
 
🚧 Supported environments: The template is only tested to compilation within [MSYS2](https://www.msys2.org/) but should also work using a native Unix or WSL system.

## Table of Content
1. [Setup](#setup)
2. [Requirements](#requirements)
3. [Compilation](#compilation)

![Image](https://drive.google.com/uc?id=1iKgnR-T8QvzZve0DJfw4KkIFrXCCxmcE)

## Setup

### 1. Clone to local repository
  - Clone this repository in your local documentation folder

### 2. Changes to be done ###
  - Change the `\projectPath` under [*defines.tex*](texdata/defines.tex)
  - Change the `\usepackage` path for minted outdata under [*preamble.tex*](texdata/preamble.tex)
  - Rename the template file as well as example sections


## Requirements

### Windows

Currently there is no direct windows support. 
It is recommended to use `MSYS2` as it also can be integrated into VS-Code.
Downloaded and installation see official MSYS Website: https://www.msys2.org/

#### Install Required packages under MSYS

MSYS uses `pacman` as packatmanager so this can be used to install the required packages

```
pacman -S make mingw-w64-x86_64-texlive-bin mingw-w64-x86_64-texlive-latex-recommended mingw-w64-x86_64-texlive-latex-extra mingw-w64-x86_64-texlive-bibtex-extra mingw-w64-x86_64-python-pygments
```

### Linux / WSL

Using a common Debian based Linux distribution `apt` can be used to install the required packages

```
sudo apt install make texlive-latex-base texlive-latex-extra texlive-bibtex-extra python3-pygments
```

> Using Arch Linux? See [pacman](#install-required-packages-under-msys)

## Compilation

Before compilation make sure the local path variables are defined like described in [Setup](#2-changes-to-be-done)

For compilation just use `make` in the root directory (Don´t blame me for the make file).
Currently it is required to run `make clean` before running `make` to ensure the correct compilation.

---

*The contributors involved assume no liability for the information provided. If you have any legal claims to the information shared or wish to report a violation, please contact smokey95.github@gmail.com*
