# BiLSTM Text Similarity

![Python](https://img.shields.io/badge/Python-3.x-blue)
![PyTorch](https://img.shields.io/badge/Framework-PyTorch-ee4c2c)
![Model](https://img.shields.io/badge/Model-BiLSTM-6f42c1)
![Task](https://img.shields.io/badge/Task-Text%20Similarity-green)

## Overview

This repository is a text similarity project based on a BiLSTM model and the STS-B dataset. It includes preprocessing, tokenizer creation, training, validation, testing, and prediction.

## Preview

![training-history](training_history.png)

## Highlights

- BiLSTM-based sentence similarity baseline
- training with early stopping and metric tracking
- tokenizer building and preprocessing pipeline
- saved checkpoints and tokenizer artifacts preserved in the repository

## Project Structure

- `train.py`: training, validation, early stopping, and metric tracking
- `predict.py`: similarity prediction
- `data_loader.py`: dataset loading and dataloader creation
- `preprocessor.py`: text preprocessing and tokenizer preparation
- `model.py`: BiLSTM similarity model definition
- `config.py`: hyperparameters and path configuration
- `STS-B/`: dataset files used during experiments

## Setup

```bash
pip install torch matplotlib scipy tqdm
```

## Usage

Train:

```bash
python train.py
```

Predict:

```bash
python predict.py
```

## Notes

- `config.py` currently contains absolute local paths for the dataset files.
- This repository is preserved more as an experiment snapshot than as a fully cleaned release.
