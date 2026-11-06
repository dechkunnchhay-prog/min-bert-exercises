# MiniBERT Exercises

## Overview

This repository contains Python exercises for learning and experimenting with MiniBERT and BERT-based sentiment classification.

The exercises use the Stanford Sentiment Treebank (SST) dataset to train and evaluate a sentiment classifier.

## Learning Objectives

By completing these exercises, students will be able to:

- Understand the architecture of BERT.
- Explore pretrained language models.
- Understand the difference between pretraining and fine-tuning.
- Implement a sentiment classification task.
- Train and evaluate a neural network using PyTorch.
- Experiment with different training configurations.

## Project Structure

```text
min_bert_exercises/
│
├── data/
│   ├── ids-sst-train.csv
│   ├── ids-sst-dev.csv
│   └── ids-sst-test-student.csv
│
├── predictions/
│   ├── classifier.py
│   ├── tokenizer.py
│   ├── bert.py
│   ├── base_bert.py
│   └── optimizer.py
│
├── requirements.txt
├── README.md
├── LICENSE
└── .gitignore
```

The hidden test labels are not included in this repository.

## Requirements

- Python
- PyTorch
- Dependencies listed in `requirements.txt`

## Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/min-bert-exercises.git
cd min-bert-exercises
```

Create a virtual environment:

```bash
python -m venv .venv
```

Activate it on Windows:

```cmd
.venv\Scripts\activate
```

Install dependencies:

```bash
python -m pip install -r requirements.txt
```

## Dataset

Place the SST dataset files inside the `data/` directory.

Required files:

- `ids-sst-train.csv`: Training dataset.
- `ids-sst-dev.csv`: Development/validation dataset.
- `ids-sst-test-student.csv`: Test dataset without ground-truth labels.

The instructor-only file `ids-sst-test_truthlabel.csv` is intentionally excluded.

## Running the Classifier

Navigate to the predictions directory:

```bash
cd predictions
```

Run the SST sentiment classifier:

```bash
python classifier.py --option pretrain --epochs 3
```

You can change the number of training epochs:

```bash
python classifier.py --option pretrain --epochs 10
```

## Exercises

Students are encouraged to:

1. Examine the BERT model implementation.
2. Explore the tokenizer and input preparation.
3. Investigate the sentiment classification architecture.
4. Experiment with different training epochs and hyperparameters.
5. Compare model performance under different configurations.
6. Analyze the generated predictions.

## License

This project is distributed under the Apache License 2.0. See the `LICENSE` file for details.

## Acknowledgements

This repository is intended for educational and research purposes. Please acknowledge the original sources of the code, pretrained models, and datasets used in your work.
