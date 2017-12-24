# Machine Learning Engineer Nanodegree
## Capstone Proposal
Li Xiaowei
24/12/2017

## Proposal
### Domain Background
In the recent years, many consumer grade products have started to deploy face recognition features. One of them is to set the name of faces in my iPhone iCloud photo library. Many beautiful memories about a specific person will be created. For example, how my daughter grew up from her born to now's four years old. When I want to view a photo about my dauther, my phone is able to show me all related photos.

I have been taking photos since my college life. It has been more than 10 years and I have accumulated more than 40k photos. I always wanted to do something to auto preprocess my photos when I import them into my computer. In this project I want to explore how to use machine learning or deep learning to perform facial recognition. More specifically, I want the faces of my family members can be tagged when a photo is imported in.

### Problem Statement
Given the photo library I have, to learn facial features on labeled data (my family members) and then auto tag the unlabeled ones. This project is not targeted for large or internet scale data.

### Datasets and Inputs
Despite I have a large photo library, not all of them are related to this project. For example, photos with no human face, photos with people other than my family members.

There ought to be some pre-processing to extract the faces from the photos first and they will be the inputs for this project.

### Solution Statement
The first step in this project will be using openCV or other possible approaches to extract the faces from my photo libraries. My photo library is in chronogical order and with proper naming about where, who and what. So it won't be too difficult to hand pick all the related faces. There will be seven people/classes for the datset.

Performing training on images is always good to start with extracting "features". So the second step will be using Google Inception V3 to extract the features. Each face photo will be represented by a vector of 4096 elements.

The dataset will be splitted into training and testing datasets at the third step.

At the fourth step, I'll explore to use KNN alone, PCA with KNN to evalute the performance of accuracy and speed. DNN will also be explored, and basically it's a transfer learning here.

The fifth step is the summary of the performance about the recognition accuracy and speed.

### Benchmark Model
Even though I have a large dataset, I don't think there is going to be many face photos. So instead of a typical train-validation-test model, I'll have a train-test model and the benchmark will be measured based on the performance of the test dataset. Probably k-fold could be explored here.

### Evaluation Metrics
The metrics will focus on accuracy and speed. Accuracy will be based on the confusion matrix of predicted and real classes. Speed will be evaluted by the system time taken by predication.

### Project Design
Unlike other projects in this MLND, which were given the input dataset. This project may require great amount of time to "create" the input dataset first.

So the entire project will have three main components. The first one is to extract faces from my photo library and manually pick/group the photos to prepare the input dateset. The second component will have few models including KNN, PCA + KNN and DNN to perform the training. Maybe other techniques will be needed on the spot. And the final component will focus on the evaluation and comparison of performance from different models.
