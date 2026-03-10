# Fake Job Posting Detection using LSTM

This project builds a Deep Learning NLP model to detect fraudulent job postings from job listing data. The model analyzes job description text and predicts whether a job posting is real or fake using a Bidirectional LSTM neural network.

Fraudulent job postings can mislead job seekers. This project demonstrates how Natural Language Processing and Deep Learning can be used to automatically identify suspicious job listings.

# Dataset

The project uses the Fake Job Postings Dataset, which contains detailed job listing information.

Features used in this project:

Job Title

Company Profile

Job Description

Requirements

Benefits

Salary Range

Target variable:

fraudulent

0 → Real Job Posting

1 → Fake Job Posting

# Project Workflow

### Data Loading

Dataset is loaded using pandas.

### Data Cleaning

Missing values are replaced with empty strings.

Columns are converted to consistent data types.

### Feature Engineering

Multiple text columns are combined into one feature.

### Text Preprocessing

Tokenization converts text into sequences.

Padding ensures fixed-length input sequences.

### Model Building

Embedding layer

Bidirectional LSTM

Dense output layer

### Model Training

Binary classification using sigmoid activation.

### Model Evaluation

Accuracy

Precision

Recall

F1-score

# Model Architecture

Embedding Layer
↓
Bidirectional LSTM (128 units)
↓
Dense Layer (Sigmoid Activation)

The Bidirectional LSTM helps the model understand context from both directions of the text.

# Model Performance

Test Accuracy: 97.76%

Classification Summary:

Class	Precision	Recall	F1-score
Real Jobs	0.98	1.00	0.99
Fake Jobs	0.90	0.63	0.74

The model performs well in detecting legitimate job postings and shows promising results in identifying fraudulent listings.

# Technologies Used

Python

Pandas

NumPy

TensorFlow / Keras

Scikit-learn

Natural Language Processing (NLP)

# Project Structure
fake-job-detection-lstm
│
├── fake_job_detection_lstm.ipynb
├── fake_job_postings.csv
└── README.md
# Future Improvements

Use Transformer models such as BERT

Improve recall for fraudulent job detection

Deploy the model as an API

Integrate with job platforms for real-time fraud detection
