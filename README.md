## Overview

HSMAD: Heterophily-Driven Spectral and Manifold Learning for Graph Anomaly Detection

## Usage

### Command-line arguments

You can run the model by executing the following command:

```bash
python main.py --dataset weibo
```

### Arguments

- `--dataset` (str): Specify the dataset to use. Available options include `yelp`, `weibo`, `amazon`, `elliptic`, and `tolokers`.
- `--run` (int): The number of runs for the experiment. Default is 1.
- `--epoch` (int): Number of epochs to train the model. Default is 1000.
- `--patience` (int): Patience for early stopping. The model will stop training if there is no improvement for this many epochs. Default is 100.
- `--order` (int): The order of filters. Default is 2.
- `--q` (float): The quantile parameter. Default is 0.5.

### Example

To run the model with the `weibo` dataset, 10 runs, 1000 epochs, patience of 100, execute:

```bash
python main.py --dataset weibo --run 10 --epoch 1000 --patience 100 --order 2 --q 0.5
```

This will train the model using the specified hyperparameters and dataset.

### Output

The results of the experiment will include:

- Performance metrics (e.g., Recall, Pecision, F1-Macro, AUC, G-Mean)
