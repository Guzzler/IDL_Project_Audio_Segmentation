# IDL Project - Audio Referring Segmentation

This repository contains the implementation for an Intro to deep learning class project based on 'Audio Referring Segmentation'. Our baseline was inspired by 
the paper titled "You Only Hear Once: A YOLO-like Algorithm for Audio Segmentation and Sound Event Detection" and our baseline has been inspired by sources of code written by the authors of the paper. [[PDF](https://www.mdpi.com/2076-3417/12/7/3293)] 

The team members behind this project:

1. Marlies Goes
2. Eesha Shetty
3. Noel Dsouza
4. Sharang Pai

We would also like to thank our mentors for this project -

1. Prakruthi Pradeep 
2. Xiang Li

The code for this project is majorly separated into 3 different folders. All code has been put into jupyter notebooks specfically so that it can be run indepedently without any problems. The notebooks have been documented and consider their own dependency management. Even so, since dependency conflicts might be an issue based on the platform of running the notebook, we have created a common `requirements.txt`. To install all requirements specifically using that one can run `pip install -r requirements.txt`


# Dataset Generation

Due to the lack of well-defined datasets for our segmentation approach, the first step of the project was to generate the dataset to set an adequate baseline. In our case we generated the dataset based on the BBC SoundDescs Dataset. We have provided the code that we used during this dataset generation in a notebook within the Dataset Generation. The dataset_generation folder consists of the notebook that has stepwise instructions to generate the dataset of audioclips. This can be easily extended to a dataset of choice by simply changing the input parameters within the notebook and the class values.

# Model Experiments

The second part of the code was setting up the model baseline and then making extensions to the model. As part of our project we ran multiple iterations over a wide set of model backbones and tried to modify components of each model. We found best results for the 3 models whose notebooks we have in the experiments folder. As mentioned before, each notebook is largely self-contained and should not require any external dependencies. They should also contain code to download the preprocessed dataset that we created for our task so that they can be run independently of the first step.

# Demo

The final folder contains a much smaller notebook that is only meant to illustrate the inference of the model on unknown data. This uses the best model and handles a few sample inputs and output audio files that were not at all part of the train or validation sets. These examples are only to indicate how well our model finally performed on the task and allow individuals to explore the final output of this project.
