# Dress-Up
This repository is changed based on the official implementation of OOTDiffusion

## Installation
1. Clone the repository

```sh
git clone https://github.com/wangg0925/dress-up
```

2. Create a conda environment and install the required packages

```sh
conda create -n ootd python==3.11
conda activate ootd
pip install -r requirements.txt
```

## Inference
1. Half-body model

```sh
cd dress-up/run
python run.py --model_path <model-image-path> --cloth_path <cloth-image-path> --scale 2.0 --sample 4
```

2. Full-body model 

> Garment category must be paired: 0 = upperbody; 1 = lowerbody; 2 = dress

```sh
cd dress-up/run
python run.py --model_path <model-image-path> --cloth_path <cloth-image-path> --model_type dc --category 2 --scale 2.0 --sample 4
```
