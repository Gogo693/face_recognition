# face_recognition

This project contains a Computer Vision model for face recognition. 

## Task
Given 2 images, it outputs 1 if those contains the face of the same person, 0 otherwise.

## Model brief description
The model is a pre-trained InceptionV3 model with an additional layer on top, then fine-tuned.

We train the model using a Triplet Loss, that is the best option to compare images at feature level to find similarities.

## Dataset
We use the LFW dataset for our experiments and we pre-process it to obtain face triplets (Anchor - Positive - Negative) for the Triplet Loss (check its implementation for details).

We use TF to import the dataset, but the code is mainly written in PyTorch.
