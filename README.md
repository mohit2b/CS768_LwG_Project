# Signet + Edge Transformer

Code for our CS768 Learning with Graphs project. 

> This repository provides the implementation for the work done as a course project in CS768 Learning with Graphs project. Our work is based on two repository, for `Edge Transformer` we refer https://github.com/luis-mueller/towards-principled-gts provided by Muller et al. 2024 and for the `Signet` we refer to https://github.com/cptq/SignNet-BasisNet provided by Lim et al. 2022. For running CLRS benchmark we refer to https://github.com/ksmdnl/clrs repository provided by Muller et al. 2024.

## Install
We utilize [`conda`](https://docs.conda.io/en/latest/) for creating the environment. For running the molecular regression benchmarks create an environment using the following command
```bash
conda create -n signet-gts python=3.10
conda activate signet-gts
```
Install all dependencies via
```bash
pip install -r /path/to/requirements.txt
```
For running the CLRS benchmark create a separate environment 
```bash
conda create -n clrs python=3.10
conda activate clrs
```
Install all dependencies via
```bash
pip install -r /path/to/clrs_requirements.txt
```

## Molecular regression
To run the Alchemy  dataset, run
```bash
python molecular-regression/alchemy.py.py root=/path/to/data/root
```
respectively, where `/path/to/data/root` specifies the path to your data folder. This folder will be created if it does not exist. For running RRWP set `rrwp=yes` in yaml file. For running Signet positional encoding set `signet_pe=yes` in yaml file.

To run the QM9 dataset, run
```bash
python molecular-regression/qm9.py root=/path/to/data/root
```
For running RRWP set `rrwp=yes` in yaml file. For running Signet positional encoding set `signet_pe=yes` in yaml file.


To run the ZINC-12K dataset, run
```bash
python molecular-regression/zinc.py root=/path/to/data/root
```
For running RRWP set `rrwp=yes` in yaml file. For running Signet positional encoding set `signet_pe=yes` in yaml file.

To run the ZINC-Full dataset, run
```bash
python molecular-regression/zinc_full.py root=/path/to/data/root
```
For running RRWP set `rrwp=yes` in yaml file. For running Signet positional encoding set `signet_pe=yes` in yaml file.

## CLRS
For running the CLRS code for Dijkstra algorithm run the following command
```bash
python -m clrs_code.examples.run --algorithms dijkstra
```