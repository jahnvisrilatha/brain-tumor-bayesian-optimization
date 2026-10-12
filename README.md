# Brain Tumor Classification Using Bayesian Optimization

## Project Overview

This project focuses on reproducing a CNN-based brain tumor classification framework using Bayesian Optimization for hyperparameter tuning. The objective is to explore suitable CNN architectures, optimize model hyperparameters, and evaluate the performance of the trained models on brain tumor MRI image datasets.

The project is based on the research paper **“Bayesian Optimization-based CNN Framework for Automated Detection of Brain Tumors” (2023)**.

##  Objectives

- Implement a flexible Convolutional Neural Network (CNN) for brain tumor image classification.
- Apply Bayesian Optimization to search for suitable CNN hyperparameters.
- Train and evaluate the optimized model on two datasets.
- Analyze classification performance using standard evaluation metrics.
- Compare experimental results with the results reported in the research paper.

##  Methodology

The project follows these major steps:

1. **Dataset Preparation:** Load the MRI image datasets, inspect the images, and prepare training, validation, and testing sets.
2. **Image Preprocessing:** Resize images to the required input dimensions and prepare them for CNN training.
3. **CNN Architecture:** Build a configurable CNN consisting of convolutional layers, filters, pooling, dropout, and dense layers.
4. **Hyperparameter Search:** Define a search space containing parameters such as the number of convolutional layers, kernel size, number of filters, dropout rate, optimizer, and learning rate.
5. **Bayesian Optimization:** Evaluate candidate configurations and use a Gaussian Process surrogate model and an acquisition function to guide the search toward promising configurations.
6. **Final Model Training:** Train the selected CNN configuration using the chosen training settings.
7. **Model Evaluation:** Evaluate the trained model on the test dataset and analyze the classification results.
8. **Performance Comparison:** Compare the experimental results with the research paper where applicable.

##  Repository Structure

```text
brain-tumor-bayesian-optimization/
│
├── BrainTumor_Dataset1_Prediction.ipynb
├── Reproduction_dataset1.ipynb
├── Reproduction_of_dataset2.ipynb
└── README.md
```

### Notebook Descriptions

- **BrainTumor_Dataset1_Prediction.ipynb:** Notebook for generating predictions on Dataset 1 using the model and workflow defined in the notebook.
- **Reproduction_dataset1.ipynb:** Implements the reproduction workflow for Dataset 1, including preprocessing, CNN configuration, Bayesian Optimization, training, and evaluation.
- **Reproduction_of_dataset2.ipynb:** Implements the reproduction workflow for Dataset 2 and evaluates the model's performance.

##  Technologies Used

- Python
- Google Colab
- TensorFlow / Keras
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Google Drive
- Git and GitHub

##  Hyperparameter Optimization

The Bayesian Optimization process explores CNN configurations using parameters such as:

- Number of convolutional layers
- Kernel size
- Number of filters
- Dropout rate
- Optimizer
- Learning rate

The search aims to identify a promising configuration based on validation performance while reducing the need to evaluate every possible combination.

##  Evaluation Metrics

The model's performance can be assessed using the following metrics, where implemented in the notebooks:

- Accuracy
- Training and validation loss
- Confusion matrix
- Precision
- Recall
- F1-score
- Matthews Correlation Coefficient (MCC)
- Cohen's Kappa

These metrics help analyze the classification performance and the types of prediction errors made by the model.

##  How to Run the Project

1. Open [Google Colab](https://colab.research.google.com/).
2. Open the required notebook from this repository.
3. Upload or connect the required datasets through Google Drive.
4. Update dataset and model paths according to your folder structure.
5. Select a suitable runtime, preferably a GPU runtime if available.
6. Execute the notebook cells in order, from dataset preparation through model evaluation.
7. Review the generated metrics, plots, confusion matrix, and comparison results.

##  Dataset and Model Files

The notebooks require the corresponding brain tumor MRI datasets. Dataset files and trained model checkpoints are not included in this repository unless explicitly uploaded.

Ensure that the dataset paths and model paths are configured correctly before running the notebooks.

##  Results

The experimental results should be taken from the completed notebook executions. Evaluation metrics can be used to assess the performance of each dataset experiment and compare the reproduced framework with the original research paper.

**Note:** Results may vary depending on the dataset, data split, hyperparameter search settings, training duration, random seeds, and computing resources.

##  Future Enhancements

- Improve the efficiency of Bayesian hyperparameter optimization.
- Experiment with additional CNN architectures.
- Improve generalization through data augmentation and regularization.
- Add visualizations for model predictions and classification errors.
- Explore explainable AI techniques to understand the model's predictions.

##  GitHub Repository

[Brain Tumor Classification Using Bayesian Optimization](https://github.com/jahnvisrilatha/brain-tumor-bayesian-optimization)
