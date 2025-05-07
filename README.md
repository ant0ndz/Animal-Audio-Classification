# Animal-Audio-Classification
This repo contains work done as part of a university project aimed at learning and appliying machine learning techniques using audio files.
It includes python notbooks used for EDA, data preprocessing, experiments containing machine learning training and testing and finally a demenstration notbook showing an example of how audio files can be processed for machine learning purposes.
Note that the code cant be run without the audio files, which are not availalbe in this repo and need to be downloaded from the compatition.

## Method:
We wanted to use audio data to classify files to an animal class, based on the animal sounds found int it.
Animal classes: Mamelia, Insecta, Aves, Amphibia.
To perform this, we split each audio into segments of 5 seconds, for each of which we perform classification using a model.
Then the entire file is then classified to the class that the majority of it's segments where classified to.
We present experiments using XGBoost as a baseline, with efficient and Resnet18 used to take advantage of spectograms for more effective classification.

## Code:
The python notebooks included are:
* EDA.ipynb - Used to explore the data and its features.
* Data Processing.ipynb - Python notebook used for the prerosess and spliting of data into train,validation and test sets.
* Experiments.ipynb - Python notebook used for runing experiments which include training and testing of different models with the goal of classifiying files to an animal class based on the audio found in it.
* Audio Preprocessing Example.ipynb - Python notebook for showing different approaches for working with audio and machine learning.

## Data
The data used is taken from from kaggles compatition named BirdCLEF+ 2025, licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/).
The data in this repo and availalbe trought the notebooks to see, is partial and preprocessed and is not the original data provided by the compatition as is.
However, the licesne of the orginigal dataset is applied also to the data in this repo.

Link to compatition: https://www.kaggle.com/competitions/birdclef-2025/data

The folder named "preprocessed data csvs" contains csvs created by "Data Processing.ipynb" for the experiments phase.


## Licensing

The code in this repository is licensed under the MIT License (see LICENSE file).

The sample dataset is derived from the BirdCLEF 2025 competition on Kaggle and is licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/). This means it may be used for non-commercial purposes only and must be attributed accordingly.
