# GENDER-PREDICTION-USING-ACOUSTIC-PROPERTIES-OF-VOICE-AND-SPEECH
 This project develops a classification model that predicts an individual's gender (male or female) using a set of diverse acoustic parameters, leveraging the power of machine learning techniques.

## Problem Statement

Create a classification model to predict an individual's gender (male or female) based on various acoustic parameters extracted from voice and speech recordings.

## Context

This dataset has been curated to distinguish between male and female voices by analyzing their acoustic characteristics. It comprises 3,168 voice samples collected from speakers of both genders. The acoustic analysis, performed using R with the seewave and tuneR packages, covers a frequency range of 0Hz to 280Hz, which encompasses the human vocal range.

## Column Descriptions

- `meanfreq`: Mean frequency (in kHz)
- `sd`: Standard deviation of frequency
- `median`: Median frequency (in kHz)
- `Q25`: First quantile (in kHz)
- `Q75`: Third quantile (in kHz)
- `IQR`: Interquantile range (in kHz)
- `skew`: Skewness
- `kurt`: Kurtosis
- `sp.ent`: Spectral entropy
- `sfm`: Spectral flatness
- `mode`: Mode frequency
- `centroid`: Frequency centroid
- `peakf`: Peak frequency (frequency with the highest energy)
- `meanfun`: Average fundamental frequency
- `minfun`: Minimum fundamental frequency
- `maxfun`: Maximum fundamental frequency
- `meandom`: Average dominant frequency
- `mindom`: Minimum dominant frequency
- `maxdom`: Maximum dominant frequency
- `dfrange`: Range of dominant frequency
- `modindx`: Modulation index

**Target Variable:**

- `label`: Gender (male or female)

## Dataset

You can access the dataset [here](https://drive.google.com/file/d/1I32cTkoT2U--InDtRjZP3BaPpUtdZ1R6/view?usp=sharing).

## Steps to Consider

1. **Data Preprocessing:**
   - Remove or handle any null values in the dataset.

2. **Data Visualization:**
   - Depict the percentage distribution of gender labels on a pie chart.

3. **Data Splitting:**
   - Split the dataset into training and testing data, with a test size of 20%.

4. **Model Building:**
   - Apply the following classifier models on the training dataset and generate predictions for the test dataset:
     - Decision Tree Classifier
     - Random Forest Classifier
     - KNN Classifier
     - Logistic Regression
     - SVM Classifier

5. **Model Evaluation:**
   - Generate confusion matrices and classification reports for each model generated in step 4.

6. **Final Report:**
   - Identify and report the model with the best accuracy among the classifiers.
