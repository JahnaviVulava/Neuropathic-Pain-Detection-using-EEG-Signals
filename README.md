# Neuropathic Pain Detection using EEG Signals and Machine Learning

## Overview

This project predicts the intensity of neuropathic pain using EEG (Electroencephalography) signals combined with patient demographic information. The system extracts statistical and frequency-domain features from EEG recordings, merges them with questionnaire data, and trains a Random Forest classifier to classify patients into High Pain and Low Pain categories.

The project also provides a simple Gradio interface where users can upload a new EEG (.gdf) file along with patient information to obtain a prediction.

---

## Features

- EEG signal preprocessing using MNE
- Statistical feature extraction
- Frequency band power extraction
- Demographic data integration
- Random Forest classification
- Feature importance visualization
- Correlation heatmap
- Gradio-based prediction interface

---

## Dataset

**Source:** Mendeley Data

**Dataset Used:**
Chronic Neuropathic Pain Dataset

The dataset contains:

- EEG recordings in `.gdf` format
- Patient demographic information
- Questionnaire responses
- Pain scores
- Medical history
- Treatment details

---

## Project Workflow

1. Load EEG (.gdf) files.
2. Preprocess EEG signals.
3. Extract statistical features:
   - Mean
   - Variance
   - Skewness
   - Kurtosis
4. Extract frequency-domain features:
   - Delta band power
   - Theta band power
   - Alpha band power
   - Beta band power
   - Gamma band power
5. Merge EEG features with questionnaire and demographic data.
6. Train Random Forest classifier.
7. Evaluate model performance.
8. Visualize feature importance and correlations.
9. Predict pain level for new patients using a Gradio interface.

---

## Technologies Used

- Python
- MNE
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- SciPy
- Gradio

---

## Machine Learning Model

Algorithm:
- Random Forest Classifier

Parameters:

- Number of Trees: 200
- Maximum Depth: 15
- Balanced Class Weights

Train-Test Split:

- Training: 80%
- Testing: 20%

---

## Extracted Features

### Statistical Features

- Mean
- Variance
- Skewness
- Kurtosis

### Spectral Features

- Delta Power
- Theta Power
- Alpha Power
- Beta Power
- Gamma Power

### Patient Information

- Age
- Gender
- Etiology of Neuropathic Pain
- Time with Neuropathic Pain
- Medical Treatment
- Previous Medication Duration
- Psychological Counseling
- Neurological Disorders
- Head Trauma History

---

## Visualizations

The project generates:

- EEG waveform plots
- FFT plots
- Pain score histogram
- Etiology distribution pie chart
- Feature importance graph
- Correlation heatmap

---

## Prediction Output

For a new patient, the system predicts:

- Pain Intensity (High or Low)
- Most similar Neuropathic Pain Etiology
- Suggested Medical Treatment (based on the closest patient profile)

---

## Installation

Install the required packages:

```bash
pip install mne numpy pandas matplotlib seaborn scipy scikit-learn gradio openpyxl shap
```

---

## Running the Project

Run the notebook:

```bash
Neuropathic_Pain_Detection.ipynb
```

The notebook will:

- Load EEG recordings
- Extract features
- Train the Random Forest model
- Display evaluation metrics
- Launch the Gradio application

---

## Project Structure

```
Neuropathic_Pain_Detection.ipynb
EEG_Features.csv
Demographics_Questionnaires_Dataset_v4.xlsx
README.md
```

---

## Future Improvements

- Deep Learning models (CNN/LSTM)
- Multi-class pain severity prediction
- Real-time EEG monitoring
- Explainable AI using SHAP
- Cloud deployment
- Larger multi-center datasets

---

## Authors

Developed as a Machine Learning project for Neuropathic Pain Detection using EEG signals and patient demographic information.

---

## Acknowledgements

- Mendeley Data for providing the Chronic Neuropathic Pain Dataset.
- MNE-Python for EEG signal processing.
- Scikit-learn for machine learning algorithms.
- Gradio for creating the interactive prediction interface.
