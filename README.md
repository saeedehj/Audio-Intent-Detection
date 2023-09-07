# Audio Intent Detection
### Problem Description

**Intent detection** is a critical task in natural language processing (NLP) and speech recognition, where the goal is to identify the underlying intention or purpose of a spoken or written statement. Accurate intent detection is crucial for voice assistants and audio-based applications as it enables them to understand and respond appropriately to user requests and commands.
This project is part of the Data Science Lab: Process and Methods at Politecnico di Torino.

### Dataset

The dataset includes audio files in WAV format.
Metadata in CSV format contains attributes like action, object, fluency level, first language spoken, current language used for work/school, gender, and age range.
An intent is defined by combining an action with an object, resulting in a label obtained through simple string concatenation (e.g., "increase" + "volume" = "increasevolume"), , which we aim to predict.

Important: Please note that only the provided dataset should be used for this project, and external datasets are not allowed.

### Proposed Approach

1. **Data Preprocessing**:
   - Standardization of audio formats and durations.
   - Feature extraction using Mel Frequency Cepstral Coefficients (MFCC) and Mel spectrogram techniques.
   - Concatenation of extracted features.
2. **Model Selection**:
   - Utilized three different models: Support Vector Machines (SVM), Random Forest, and Convolutional Neural Networks (CNN).
3. **Hyperparameter Tuning**:
   - Optimized hyperparameters for SVM and Random Forest models through grid search.
   
### Evaluation Metric

Submissions will be evaluated based on Accuracy.

### Results

- SVM achieved an accuracy of approximately 0.49645 with the best configuration.
- Random Forest achieved an accuracy of approximately 0.408 with the best configuration.
- CNN outperformed other models with a training accuracy of around 0.977 and a public score of 0.9.

### Discussion

- The CNN approach yielded significantly better results compared to SVM and Random Forest.
- Considerations for further improvements include exploring alternative feature extraction approaches, multi-task classification, and addressing class imbalance in the dataset.



**Keywords**: Audio classification, Machine learning, SVM, Random Forest, CNN


