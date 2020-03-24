# Sentiment Analysis with PyTorch (SageMaker Deployment Project)

This project implements RNNs vis PyTorch to identify whether a movie review is positive or negative. The training and testing were done with the [IMDB dataset](http://ai.stanford.edu/~amaas/data/sentiment/). The model is then deployed via Amazon Sagemaker. A simple webapp is written to interact with the model via an API that is made accessible through AWS Lambda.

## Important notice

This project was done as a part of Udacity's Machine Learning Engineer Nanodegree. All the rights belong to the authors of the project.

## Setup
The notebook here is intended to be executed using Amazon's Sagemaker platform. For more detail, please read the [README](https://github.com/udacity/sagemaker-deployment/tree/master/README.md) in the root directory for instructions on setting up a SageMaker notebook.

## Folders and Files

- `Sagemaker-Project.ipynb` : This is the main notebook where the data is preprocessed, and the model is implemented, deployed and tested.
- `train` : This folder contains the `model.py` file that defines the RNN and the `train.py` file that defines the train function.
- `serve` : This folder contains the `model.py` file that defines the RNN, the `predict.py` file that defines the predict function and the `utils.py` that contains the utility functions to preprocess the data.
- `website` : This folder contains the `index.html`, which is a simple webapp that interacts with the model via a public API. **Please note that the endpoint was already shut down and you will have to run the notebook yourself for the webapp to be working.**
