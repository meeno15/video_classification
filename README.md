# video_classification
This repository contains code for a football video classification project using a Long Short-Term Memory (LSTM) model. The goal of the project is to classify trimmed football videos into three categories: fouls, scoring, and red cards.

## Introduction
Video classification plays a crucial role in understanding and analyzing sports footage. This project focuses on classifying football videos into different categories based on their content. By using an LSTM-based architecture, the model can effectively capture the temporal dependencies and nuances present in the trimmed football videos.

The code in this repository implements a sequence model using Keras and TensorFlow libraries. It includes data preprocessing, model training, and evaluation steps.

## Dataset
The football video dataset used in this project was obtained from Kaggle. You can access the dataset using the following link: Football Match Actions Video Dataset.`https://www.kaggle.com/datasets/itarek898/football-match-actions-video-dataset` The dataset contains trimmed football videos that are labeled with fouls, scoring, and red cards actions.

Before using the dataset, it is recommended to preprocess the data and split it into training, validation, and test sets. To assist with the preprocessing steps, a Jupyter Notebook file named dataset.ipynb has been included in this repository. This notebook provides code and instructions for performing basic pre-processing tasks, such as data cleaning, feature extraction, and splitting the dataset into training, validation, and test sets.

Make sure to run the dataset.ipynb notebook to preprocess the data before running the code in the main project files.

## Model Architecture
The football video classification model used in this project is based on LSTM networks. It consists of bidirectional LSTM layers followed by a single LSTM layer. Batch normalization is applied to normalize the output, and fully connected layers with dropout regularization are used for classification. The model is trained using the Adam optimizer with a learning rate of 0.001 and sparse categorical cross-entropy as the loss function.

For a more detailed explanation of the model architecture, please refer to the code comments in the get_sequence_model() function.

## Results
After running the experiment, the model achieved an accuracy of 91% on the test dataset, showcasing its effectiveness in classifying football videos. The confusion matrix also demonstrated reliable performance across the fouls, scoring, and red cards categories.
<img width="991" alt="1" src="https://github.com/meeno15/video_classification/assets/57276152/2e574ae4-c226-45aa-9e55-4abb7794a515">
<img width="850" alt="2" src="https://github.com/meeno15/video_classification/assets/57276152/30e7a59d-589e-4889-beaa-dcb6af6fca18">
<img width="647" alt="3" src="https://github.com/meeno15/video_classification/assets/57276152/9f1ea5f9-28fe-4bab-9f33-8fdf4ebaeec6">



**The project is still ongoing, with the team working on cloning a voice to these videos. This voice cloning aims to provide commentary or additional audio context to enhance the viewing experience.**

## Contributing
The project is done by me and two other friends. Contributions to this project are welcome! If you have any suggestions, bug fixes, or additional features, please submit a pull request. For major changes, please open an issue first to discuss the proposed changes.



