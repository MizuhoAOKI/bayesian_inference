[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Rye](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/rye/main/artwork/badge.json)](https://rye.astral.sh)

# Bayesian Inference

## Dependency

- [python](https://www.python.org/)
  - version 3.10 or higher is recommended.

- [rye](https://rye.astral.sh/)
  - seting up python environment easily and safely.
  - `notebook`, `numpy`, `matplotlib` are needed to run all scripts in this repository.

- [ffmpeg](https://ffmpeg.org/)
  - mp4 movie writer
  - <details>
    <summary>installation details</summary>

    - For Ubuntu Users
        - `sudo apt-get update`
        - `sudo apt-get -y install ffmpeg`
    - For Windows Users
        - Install [scoop](https://scoop.sh/)
        - `scoop install ffmpeg`
    - For macOS Users
        - Install [homebrew](https://brew.sh/)
        - `brew install ffmpeg`
    - Check the official website if necessary
        - https://ffmpeg.org/

    </details>

## Setup
```sh
git clone https://github.com/MizuhoAOKI/bayesian_inference.git
cd bayesian_inference
rye sync
```

## Usage

### [Ex. 1] Bayesian Inference with SVGD
Run bayesian inference using SVGD.  
The ground truth probability distribution function is a mixture gaussian model.

```sh
cd bayesian_inference
rye run jupyter notebook notebooks/svgd.ipynb
```

### [Ex. 2] Bayesian Inference with Stein transport

COMING SOON ...

## References
- [Qiang Liu, Dilin Wang, "Stein Variational Gradient Descent: A General Purpose Bayesian Inference Algorithm", NIPS, 2016.](https://arxiv.org/abs/1608.04471)
