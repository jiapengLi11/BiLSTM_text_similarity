# BiLSTM Text Similarity

## Overview

This repository is a text similarity project based on a BiLSTM model and the STS-B dataset. It includes preprocessing, tokenizer creation, training, validation, testing, and prediction.

## Tech Stack

- Python
- PyTorch
- BiLSTM
- Matplotlib / SciPy / tqdm

## Project Structure

- `train.py`: training, validation, early stopping, and metric tracking
- `predict.py`: similarity prediction
- `data_loader.py`: dataset loading and dataloader creation
- `preprocessor.py`: text preprocessing and tokenizer preparation
- `model.py`: BiLSTM similarity model definition
- `config.py`: hyperparameters and file-path configuration
- `STS-B/`: dataset files used during experiments
- `training_history.png`: exported training curve

## Existing Artifacts

The repository currently still contains local model outputs:

- `chinese_similarity_model.pth`
- `chinese_similarity_model_best.pth`
- `chinese_tokenizer.pkl`

## Setup

```bash
pip install torch matplotlib scipy tqdm
```

## Usage

Train and evaluate the model:

```bash
python train.py
```

Run prediction:

```bash
python predict.py
```

## Notes

- `config.py` currently contains absolute local paths for the dataset files.
- This repository is best viewed as a preserved experiment project rather than a fully cleaned release.
- A useful next improvement would be adding a dedicated `requirements.txt` and replacing absolute paths with relative ones.
