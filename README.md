# Evaluating the Impact of Compression Techniques on the Robustness of CNNs under Natural  Corruptions
This repository contains all the code used in the design of this article.

## Notebook Organization

The notebooks are organized as follows:

### `Train_and_Evaluate.ipynb`
- Contains all the code used for training the models.
- Performs evaluation of the models **before conversion to TFLite**.
- Handles the conversion of trained models to the **TFLite format**.

### `Evaluate_TFlite.ipynb`
- Performs evaluation of models **already converted** to the TFLite format.

### `Calculate_Metrics.ipynb`
- Computes the following evaluation metrics:
  - **mCE (mean Corruption Error)**
  - **Accuracy**
  - **Compression Rate**

### `results/` Folder

The `results` folder contains the outputs obtained for **CIFAR-10** and **CIFAR-100** for each evaluated model. Specifically, it includes:

- **Training history** for each model.
- **Evaluation results** under various corruption types considered in this work.

These corruption results are used to compute the **mCE (mean Corruption Error)** metric, which is calculated in the `Calculate_Metrics.ipynb` notebook.

### Trained Models

The trained models are **not yet available in this repository** due to their large size (several gigabytes) and the number of different versions.  

However, a download link will soon be provided to access all trained models.

In the meantime, the notebooks mentioned above allow full **reproducibility of the results**, including training, evaluation, and metric calculation.

### CIFAR-10-C and CIFAR-100-C
Hendrycks, D., & Dietterich, T. (2019). *Benchmarking Neural Network Robustness to Common Corruptions and Perturbations*. International Conference on Learning Representations (ICLR). [Link](https://openreview.net/forum?id=HJz6tiCqYm)

The corrupted versions of the **CIFAR-10** and **CIFAR-100** datasets used in this work can be found at the following link:

🔗 [https://github.com/hendrycks/robustness](https://github.com/hendrycks/robustness)

These datasets include various natural corruption types and are used to compute the **mCE (mean Corruption Error)** metric.
