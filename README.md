# Mental Health Status Detection From Statements Using Natural Language Processing and Neural Networks

## Project Overview

This project presents an automated Mental Health Status Detection system that classifies written statements into different mental health categories using Natural Language Processing (NLP) and Deep Learning techniques. The objective is to support early identification of mental health conditions by analyzing textual expressions shared through digital platforms.

The system processes user-generated text and predicts one of five psychological states:

* Anxiety
* Depression
* Stress
* Bipolar Disorder
* Normal

The project demonstrates how machine learning can assist mental health professionals by providing scalable screening support while emphasizing that such systems are not replacements for clinical diagnosis.

---

## Objectives

The primary objectives of this project are:

1. To identify linguistic patterns associated with different mental health conditions.
2. To develop a deep learning model capable of classifying mental health states from text.
3. To evaluate model performance across multiple psychological categories.
4. To investigate challenges such as class imbalance and misclassification.
5. To explore the practical and ethical implications of AI-based mental health screening systems.

---

## Dataset

The dataset used in this project was obtained from Kaggle and contains approximately 40,000 labeled textual statements collected from online platforms.

Dataset Link:

https://www.kaggle.com/datasets/imtkaggleteam/mental-health

### Dataset Classes

* Anxiety
* Bipolar
* Depression
* Normal
* Stress

The dataset was divided into training, validation, and testing subsets while maintaining class distribution.

---

## Technologies Used

### Programming Language

* Python

### Libraries and Frameworks

* TensorFlow
* Keras
* NumPy
* Pandas
* Scikit-learn
* NLTK
* Matplotlib
* Seaborn

### Development Environment

* Jupyter Notebook
* Google Colab

---

## Methodology

### 1. Data Preprocessing

The textual data was cleaned and standardized using the following steps:

* Lowercase conversion
* Removal of URLs and special characters
* Tokenization
* Stop-word removal
* Lemmatization
* Sequence padding

### 2. Feature Representation

Text statements were converted into numerical representations using:

* Tokenization
* Vocabulary indexing
* Sequence encoding
* Padding for fixed-length input sequences

### 3. Model Architecture

The proposed model consists of:

* Embedding Layer
* Bidirectional Recurrent Neural Network (Bi-RNN/Bi-LSTM)
* Dropout Layer
* Dense Hidden Layer
* Softmax Output Layer

The Bidirectional architecture captures contextual information from both forward and backward directions, improving understanding of sentence meaning.

### 4. Model Training

The model was trained using:

* Adam Optimizer
* Categorical Cross-Entropy Loss
* Mini-batch Gradient Descent

Hyperparameters were tuned to achieve optimal performance.

---

## Hyperparameter Configuration

| Parameter           | Selected Value |
| ------------------- | -------------- |
| Embedding Dimension | 128            |
| RNN Units           | 128            |
| Dropout Rate        | 0.3            |
| Batch Size          | 64             |
| Learning Rate       | 0.001          |
| Epochs              | 10             |

---

## Results

The final model achieved approximately:

* Accuracy: 80%
* Precision: 78%
* Recall: 79%
* F1-Score: 78%

### Class-wise Performance

| Class      | F1-Score |
| ---------- | -------- |
| Normal     | 0.81     |
| Anxiety    | 0.79     |
| Depression | 0.79     |
| Stress     | 0.74     |
| Bipolar    | 0.61     |

The model performed best on frequently represented classes while lower performance was observed for the underrepresented Bipolar category.

---

## Key Findings

* Mental health conditions exhibit identifiable linguistic patterns.
* Bidirectional neural networks effectively capture contextual information in text.
* Class imbalance significantly affects prediction performance.
* NLP-based systems can support large-scale mental health screening.

---

## Ethical Considerations

This project acknowledges several ethical concerns:

* User privacy and data protection.
* Potential algorithmic bias.
* Risk of misuse for surveillance purposes.
* Need for human oversight in clinical environments.
* Importance of transparency and explainability.

The developed system is intended only as a supportive screening tool and not as a replacement for professional mental health assessment.

---

## Future Work

Future improvements may include:

* Transformer-based architectures such as BERT and RoBERTa.
* Explainable AI techniques.
* Multilingual datasets.
* Real-time monitoring systems.
* Clinical validation using expert-labeled data.

---

## Project Structure

```text
Mental-Health-Detection/
│
├── dataset/
├── MENTAL_HEALTH_STATUS_DETECTION  code file
├── abhishikthaathota23096965 report.docx
├── README.md
```

---

## Author

**ABHISHIKTHA ATHOTA**
Student ID: 23096965
MSc Data Science
University of Hertfordshire

Supervisor: Avinash Yadav

---

## Conclusion

This project demonstrates the feasibility of using Natural Language Processing and Neural Networks for mental health status detection. The developed model successfully classifies psychological states from textual statements with approximately 80% accuracy and highlights the potential of AI-assisted mental health screening systems for future healthcare applications.
