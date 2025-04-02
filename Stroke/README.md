# Stroke Prediction  

**Stroke Prediction Using Deep Learning**   

## Overview  
This project implements a **deep learning-based stroke prediction model** to classify whether a person is at risk of having a stroke. The model is built using **TensorFlow/Keras** and trained on health and demographic data.  

## Features 
- Exploratory Data Analysis (EDA) with Seaborn and Matplotlib.
- Data preprocessing including categorical encoding and normalization.
- Handling class imbalance using SMOTE.
- Deep Learning model built with TensorFlow/Keras.
- Model training with early stopping to prevent overfitting.

## Exploratory Data Analysis (EDA)
![EDA1](https://github.com/sameeksha15/Deep_Learning/blob/main/Stroke/Images/Untitled.png)
![EDA2](https://github.com/sameeksha15/Deep_Learning/blob/main/Stroke/Images/Untitled1.png)
![EDA3](https://github.com/sameeksha15/Deep_Learning/blob/main/Stroke/Images/Untitled2.png)

## Model Architecture

The model consists of:

    Input Layer: 14 neurons with ReLU activation.
    Hidden Layers:
        7 neurons with ReLU activation.
        3 neurons with ReLU activation.
    Output Layer: 1 neuron with Sigmoid activation (Binary Classification).

## Training and Optimization
- Loss Function: Binary Crossentropy.
- Optimizer: Adam.
- Batch Size: 16.
- Early Stopping: Stops training if validation loss doesn't improve for 17 epochs.

![ValCurve](https://github.com/sameeksha15/Deep_Learning/blob/main/Stroke/Images/curve.png)

### 📂 Sample Data  
```plaintext
| Gender | Age  | Hypertension | Heart Disease | Ever Married | Work Type | Residence Type | Avg Glucose Level | BMI  | Smoking Status    | Stroke |
|--------|------|-------------|---------------|--------------|-----------|----------------|-------------------|------|------------------|--------|
| Male   | 58.0 | 1           | 0             | Yes          | Private   | Urban          | 87.96             | 39.2 | never smoked     | 0      |
| Female | 70.0 | 0           | 0             | Yes          | Private   | Rural          | 69.04             | 35.9 | formerly smoked  | 0      |
| Female | 52.0 | 0           | 0             | Yes          | Private   | Urban          | 77.59             | 17.7 | formerly smoked  | 0      |

```
## 🛠️ Setup  

Clone the repository:  
```bash
git clone https://github.com/sameeksha15/Deep_Learning.git
cd Stroke
