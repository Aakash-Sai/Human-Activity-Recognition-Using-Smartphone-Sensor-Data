
## Project Overview
This project sheds light on the fascinating realm of human activity recognition by harnessing the power of smartphone sensor data. This innovative approach leverages Bidirectional Long Short-Term Memory (BiLSTM) network to predict a user's activities like walking, laying, standing, walking upstairs/downstairs and sitting as performed by the user. 

## Features
This comprehensive project comprises of four pivotal modules: Data Acquisition, Pre-processing, Feature Extraction, and Classification. 
* The Data Acquisition module processes sampling signals obtained from the [UCI HAR Dataset](https://archive.ics.uci.edu/dataset/240/human+activity+recognition+using+smartphones).
* In the Pre-processing module the primary goal was to normalize and reduce noise from the data, ensuring that subsequent data mining algorithms yield accurate and reliable results.
* The Feature Extraction module is dedicated to selecting the most relevant features and eliminating redundant data. We used the Fischer Score here.
* The next and final module is the classification module where we use the data to classify it into activities such as standing, sitting, sleeping, and walking upstairs and downstairs using the BiLSTM algorithm.

## Technologies used
* Python 
* TensorFlow 
* Scikit Learn 
* Google Colab

## Results & Findings
The model performed quite well with an overall accuracy of 81.30%.
We observed that our model's loss exhibits step-like, repeating activity. It might be that the model observed recurrent behavior in the input data it received.
Another useful finding was that the model manages to accurately predict the 'laying' activity, but is confused between the activities such as 'walking upstairs' and 'walking downstairs'.
