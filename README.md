# Medical Assistant System

## Introduction
This project is designed to intake symptoms reported by users, predict potential diseases, and then recommend the most appropriate specialist doctors based on user ratings. It is especially beneficial for individuals who may not have extensive medical knowledge but need guidance on whether and when to consult a doctor. By accurately predicting diseases from symptoms and linking these to specialized doctors, the system ensures that patients can seek timely and relevant medical advice, reducing unnecessary hospital visits and allowing for more targeted healthcare interventions.

## Overview
The system takes symptoms from users, predicts possible diseases, and then recommends corresponding specialist doctors based on the highest user satisfaction scores. It aims to simplify and improve the accuracy of self-diagnosis processes and streamline the process of finding the right medical professional.

## Dataset
The dataset used in this project consists of disease and symptom data scraped from the internet:
- **Diseases and Symptoms:** Data was initially scraped from the National Health Portal of India and further enriched by extracting information from various Wikipedia pages.
- **Doctor Profiles:** Doctor data, including specialties and ratings, was sourced from a comprehensive dataset available on [Kaggle](https://www.kaggle.com/datasets/umarzafar/pakistani-doctors-profiles-dataset), which details Pakistani doctors' profiles.

## Disease to Symptom Mapping
Mapping between diseases and symptoms was generated using advanced natural language processing techniques, including GPT-3.5, ensuring a high level of accuracy and relevance.

## System Workflow
- **Data Collection:** Collection of Data from various sources.
- **Symptom Input:** Users input their symptoms into the system.
- **Disease Prediction:** The system employs machine learning models to predict potential diseases based on the input symptoms.
- **Doctor Recommendation:** Based on the predicted diseases, the system recommends doctors specializing in the relevant medical fields, prioritizing those with the highest user satisfaction ratings.

## Requirements
Before running the system, ensure all necessary dependencies are installed. Please refer to the `requirements.txt` file included in the repository, which lists all the libraries and their versions needed for the project. To install these dependencies, run the following command in your virtual environment:  
pip install -r requirements.txt



## Running the System
To operate the system:
1. **Notebook Use:** Open the `Doctor_Recommendation.ipynb` in Google Colab (recommended) or any Jupyter environment.
2. **Execution:** Run all cells in the notebook. Users will be prompted to input their symptoms at required steps.
3. **Dependencies:** Ensure all dependencies are installed as specified in the notebook, particularly the googlesearch library if running outside Google Colab to avoid potential issues.

## Results
The effectiveness of the system was validated by comparing its disease predictions with outputs from established medical databases like WebMD’s Symptom Checker. Our models, specifically K-Nearest Neighbor and Decision Tree, achieved an accuracy rate of up to 91.29%.

