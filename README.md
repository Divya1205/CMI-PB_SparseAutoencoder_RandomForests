# Workflow Explanation

This repository contains a set of Jupyter notebooks to handle and preprocess data efficiently. Below is an explanation of the workflow and purpose of the included notebooks:

## **1. Downloading the Data**

- **Notebook**: `DownloadData.ipynb`
- **Purpose**: This notebook is used to download all the necessary data required for analysis. It ensures that all datasets are collected and organized in the appropriate directories for further processing.

## **2. Reading and Processing the Data**

- **Notebook**: `ReadingData.ipynb`
- **Purpose**: This notebook:
  - Reads all the downloaded data files efficiently.
  - Processes the data to create training and testing datasets for antibody titer analysis.
  - Saves the following CSV files:
    - `abtiter_data_X_train.csv`: Features for training.
    - `abtiter_data_X_test.csv`: Features for testing.
    - `abtiter_data_y_train.csv`: Labels for training (not available for the test set).

## **3. Task IGg_PT Folder**

- **Location**: `CMI-PB_SparseAutoencoder_RandomForests\Tasks\Task_IGg_PT`
- **Contents**: This folder contains:
  - `Data`: Includes the processed datasets for the IGg prediction task.
  - `Scripts`: Contains code for model training and prediction.
    - **Key Script**: `SparseAutoencoderRegression_v1.ipynb` is the main script used for running all predictions.
  - `Results`: Stores the outputs and results from the prediction models.

## **Key Notes**


- The training labels (`y_train`) are only provided for the training set.
-Submitted predictions only for antibody titer task. But preprocessed the data for monocyte task as well

