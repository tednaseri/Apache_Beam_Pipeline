# Apache_Beam_Pipeline

<p align="justify">This repository includes an introductory projects for building an <strong>Apache Beam Pipeline</strong>.
To deploy this pipeline, a project is defined within Google Clouds Platform. Then test dataset is considered as a real-time data. 
So, initially they are uploaded to the google storage. It should be noted that the trained ML model (multinomial naive bayes) is also uploaded
to the google storage. Then, during the running of the Apache Beam Pipeline, the real-time data and machine learning model will be loaded from the GCP.</p>

### Pipeline:
It is made of 4 parts: 
1- Reading data from GCP<br>
2- Applying text preprocess
3- Loading trained model from GCP and applying on a given input
4- Writing result to the GCP.

# Files and Folders in this Repository:
### Code Folder:
There are two files inside this folder:
1) Classifier_model.ipynb: It includes reading input file, applying preprocess and machine learning model. The output of this file are trained model and test dataset
which is unseen data to our ML model.
2) Pipeline.ipynb: This file includes the implementation of Apache Beam Pipeline

### Data:
This folder includes the source dataset of the project that can be downloaded from the UCI GitHub repository.

### Real_Time_Data:
1- This folder includes the test data set which is already uploaded to the GCP. 
2- Also, it includes the prediction result which is obtained through the running of the Apache Beam Pipeline over test dataset.

### Trained_mode:
The optimized ML model is saved in this folder.
