# ClimSav Usage Guide

This document provides detailed instructions on how to use ClimSav, including installation, data preparation, and model training.

## Installation

1. **Install Snakemake**: Follow the [Snakemake Installation Guide](https://snakemake.readthedocs.io/en/stable/getting_started/installation.html) for installation instructions.

2. **Download and Install ClimSav**: Clone the repository and install the necessary dependencies.

    ```bash
    git clone https://github.com/ndugu-nelson/climsav.git
    cd climsav
    pip install -r requirements.txt
    ```

## Data Preparation

### Downloading Data

1. **CMIP6 Data**: Download and regrid CMIP6 datasets. Example command:

    ```bash
    snakemake all --configfile config_2m_temperature.yml --cores 8
    ```

2. **ERA5 Data**: Download ERA5 data and preprocess:

    ```bash
    python src/data_preprocessing/nc2np_equally_era5.py \
        --root_dir /mnt/data/5.625deg \
        --save_dir /mnt/data/5.625deg_npz \
        --start_train_year 1979 --start_val_year 2016 \
        --start_test_year 2017 --end_year 2019 --num_shards 8
    ```

### Understanding Data Resolution

- **5.625° Data**: Coarser resolution, suitable for global-scale modeling.
- **1.40625° Data**: Finer resolution, provides detailed local climate information.

## Training

### Pretraining

To pretrain ClimSav, use:

```bash
python src/ClimSav/pretrain/train.py --config <path/to/config>

