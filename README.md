# README.md

## Oreum Recruit Project `oreum_recruit_exercises`

2022Q2

Stripped-down / skeleton project to host interactive Notebooks used for 
technical recruitment. 
**This contains exercises only, worked examples are in another repo.**

This uses a relatively standard / barebones install of basic data manipulation 
packages including `numpy`, `scipy`, `pandas`, `matplotlib` etc. Refer to 
[oreum_template](https://github.com/oreum-industries/oreum_template)
if you want to add any standard directory structures back in

### Contents

1. Instructions for Manual Installation of the Environment

### Notes

+ We use a scientific Python stack for scripting / package development and
interactive Jupyter Notebooks for reproducible research
+ The project is hosted publicly on Oreum Industries Github at
[oreum_recruit_exercises](https://github.com/oreum-industries/oreum_recruit_exercises)
+ Project began on 2022-06-12
+ The README.md is MacOS and POSIX oriented
+ See LICENSE.md for licensing and copyright details
+ See CONTRIBUTORS.md for list of contributors

---

## 1. Instructions for Manual Installation of the Environment

This project is intended for interactive development and execution and is
manually installed.

### 1.1 Pre-req: Continuum Anaconda Python 3.9.* 64bit

Download latest from:
[https://www.continuum.io/downloads](https://www.continuum.io/downloads)

### 1.2 Git clone the repo

Assumes `git` already installed

```zsh
$> git clone https://github.com/oreum-industries/oreum_recruit_exercises
$> cd oreum_recruit_exercises
```

### 1.3 Create virtual environment

Notes:

+ This compound method uses `conda` for main environment and packages,
and `pip` for selected additional packages handled better by pip than conda.
+ See [cheat sheet of conda commands](https://conda.io/docs/_downloads/conda-cheatsheet.pdf)
+ Use `direnv` on MacOS to automatically run file `.envrc` upon directory open

#### 1.3.1 Main environment and packages using conda

```zsh
$> conda update -n base -c defaults conda
$> conda env create --file condaenv_oreum_recruit_exercises.yml
$> conda activate oreum_recruit_exercises
```

### 1.4 Configs for Local Development

Some notes to help configure local development environment

#### 1.4.1 Git config `~/.gitconfig`

```yaml
[user]
    name = <YOUR NAME>
    email = <YOUR EMAIL ADDRESS>
```

#### 1.4.2 Jupyter config

Assumes `jupyter` installed, sets defaults

```zsh
$> jupyter notebook --generate-config
$> jupyter qtconsole --generate-config
$> jupyter nbconvert --generate-config
```

### 1.5 Misc

None


---
Oreum OÜ &copy; 2022
