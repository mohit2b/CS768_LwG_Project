# Signet + Edge Transformers

Code for our CS768 Learning with Graphs project. 

> This repository provides the implementation for the work done as a course project in CS768 Learning with Graphs project. Our work is based on two repository, for `Edge Transformer` we refer https://github.com/luis-mueller/towards-principled-gts provided by Muller et al. 2024 and for the `Signet` we refer to https://github.com/cptq/SignNet-BasisNet provided by Lim et al. 2022.

## Install
We utilize [`conda`](https://docs.conda.io/en/latest/) for creating the environment. After installing it create the environment using the following command
```bash
conda create -n signet-gts python=3.10
conda activate signet-gts
```
Install all dependencies via
```bash
pip install -r /path/to/requirements.txt
```