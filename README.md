## Prerequisites

This repository is tested under the following system settings:

- Ubuntu 16.04
- Python 3.7 (Anaconda/Miniconda reconmmended)
- Pytorch 1.0.0 or above
- CUDA 9.0 or above


## Install

### Local

For most of the users, you may consider install ADN locally on your machine with the following steps.

- Install [Pytorch](https://pytorch.org/get-started/locally/) and [Anaconda](https://www.anaconda.com/distribution/#download-section)/[Miniconda](https://docs.conda.io/en/latest/miniconda.html)
  - Anaconda/Miniconda installation is optional. If not installed, you may have to install some dependent python packages manually.
- Install Python dependencies.

```cmd
pip install -r requirements.txt
```

### Natural image

- Our code assumes you have prepared your natural image dataset as following.

```cmd
your_dataset
├── test
│   ├── artifact # a folder containing all the testing images with artifact
│   └── no_artifact # a folder containing all the testing images without artifact
└── train
    ├── artifact # a folder containing all the training images with artifact
    └── no_artifact # a folder containing all the training images without artifact
```

## Demo



## Train and Test

- Configure the training and testing. We use a two-stage configuration for ADN, one for the default settings and the other for the run settings.
  - The default settings of ADN can be found at `config/adn.yaml` which is not subject to be changed. When users do not provide the values for a specific setting, the default setting in this file will be used.
  - The run settings can be found at `runs/adn.yaml`. This is where the users provide specific settings for ADN's training and testing. Any provided settings in this file will override the default settings during the experiments. **By default, the settings for training and testing ADN with DeepLesion, Spineweb and natural image datasets are provided in** `runs/adn.yaml`.

- Train ADN with  a natural image dataset. The training results (model checkpoints, configs, losses, training visualizations, etc.) can be found under `runs/run_name/` where `run_name` can be  `nature_image`

```cmd
python train.py nature_image
```

- Test ADN with DeepLesion, Spineweb datasets or a natural image dataset. The testing results (evaluation metrics and testing visualizations, etc.) can be found under `runs/run_name/` where `run_name` can be `nature_image`.

```cmd
python test.py nature_image
```
