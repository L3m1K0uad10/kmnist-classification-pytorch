# KMNIST Classification with PyTorch

This repository demonstrates the use of PyTorch to classify the [KMNIST](https://github.com/rois-codh/kmnist) dataset using various models. The models range from simple linear models to more complex convolutional neural networks (CNNs), showcasing the improvement in performance as the models increase in complexity.

## Models

- **Model 0 (Baseline Linear Model)**: A simple linear model with two layers, trained for 3 epochs with learning rate 0.1.
- **Model 1 (Extended Linear Model)**: A linear model with additional ReLU activation functions, trained for 5 epochs with learning rate 0.01.
- **Model 2 (CNN with One Block)**: A convolutional model with one convolutional block, trained for 25 epochs with learning rate 0.01.
- **Model 3 (CNN with Two Blocks)**: A convolutional model with two convolutional blocks, trained for 28 epochs with learning rate 0.001.

Each model uses **CrossEntropyLoss** as the loss function and **SGD** as the optimizer.

## Performance

| Model Name       | Loss     | Accuracy  |
|------------------|----------|-----------|
| **Model 0**      | 1.098    | 67.46%    |
| **Model 1**      | 0.987    | 70.26%    |
| **Model 2**      | 0.425    | 88.65%    |
| **Model 3**      | 0.392    | 91.46%    |

## Dataset

The KMNIST dataset is used for this classification task. It is available at [KMNIST GitHub Repository](https://github.com/rois-codh/kmnist). Alternatively, you can load the dataset directly within the notebook.

## Running the Notebook

You can open the Jupyter notebook `KMNIST_Models.ipynb` and run the cells to train and evaluate the models.

```bash
jupyter notebook notebooks/KMNIST_Models.ipynb

