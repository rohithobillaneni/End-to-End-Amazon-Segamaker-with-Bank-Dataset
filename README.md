# End-to-End-Amazon-Segamaker-with-Bank-Dataset

# Bank Application with SageMaker XGBoost

This repository contains code for building, training, and deploying a machine learning model using Amazon SageMaker XGBoost algorithm for a bank application dataset.

## Table of Contents
1. [Introduction](#introduction)
2. [Prerequisites](#prerequisites)
3. [Getting Started](#getting-started)
4. [Steps to Follow](#steps-to-follow)
5. [Deleting Endpoints](#deleting-endpoints)

## Introduction

In this project, we use Amazon SageMaker, a fully managed service that enables developers and data scientists to quickly and easily build, train, and deploy machine learning models at any scale.

## Prerequisites

Before you begin, ensure you have the following prerequisites:
- An AWS account with appropriate permissions to create SageMaker resources.
- Python 3.x installed on your local machine.
- Basic knowledge of machine learning concepts and AWS services.

## Getting Started

1. Clone this repository to your local machine.
2. Make sure you have the necessary AWS credentials configured.
3. Install required Python libraries using `pip install -r requirements.txt`.
4. Follow the steps below to build, train, and deploy the machine learning model.

## Steps to Follow

### Importing Important Libraries

- Ensure necessary libraries like `sagemaker`, `boto3`, and `pandas` are imported.
- Set up AWS credentials and create an S3 bucket.

### Downloading the Dataset and Storing in S3

- Download the dataset from the provided URL and store it in S3.
- Split the dataset into train and test data.
- Save train and test data into S3 buckets.

### Building Models XGBoost - Inbuilt Algorithm

- Use SageMaker's XGBoost container to build the model.
- Initialize hyperparameters and create a SageMaker estimator.
- Fit the estimator using the train and test data.

### Deploy Machine Learning Model as Endpoints

- Deploy the trained model as an endpoint using SageMaker.
- Make predictions on the test data using the deployed endpoint.

### Prediction of the Test Data

- Use the deployed endpoint to make predictions on the test data.
- Evaluate the model performance using a confusion matrix.

### Deleting The Endpoints

- Delete the deployed endpoint and clean up resources.

## Deleting Endpoints

- Ensure to delete the deployed endpoints and clean up S3 resources to avoid unnecessary charges.

