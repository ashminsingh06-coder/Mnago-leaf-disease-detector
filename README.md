# Mango-leaf-disease-detector
# 🥭 Mango Leaf Disease Detection Using Deep Learning

## 📌 Project Overview

Mango is one of the most important fruit crops, and leaf diseases can significantly affect crop health and yield. Early and accurate identification of these diseases can help farmers take preventive action before the infection spreads.

This project uses **Deep Learning and Computer Vision** to automatically classify mango leaf images into different disease categories. Multiple pre-trained Convolutional Neural Network (CNN) models were implemented and compared to identify the most effective model for mango leaf disease detection.

The trained models are integrated into an interactive **Streamlit web application**, allowing users to upload an image of a mango leaf and receive a predicted disease class along with the model's confidence score.

---

## 🎯 Objectives

* Develop an automated system for mango leaf disease classification.
* Apply **Transfer Learning** using state-of-the-art CNN architectures.
* Train and evaluate multiple Deep Learning models.
* Compare model performance using different evaluation metrics.
* Build a user-friendly web interface using Streamlit.
* Provide disease prediction and confidence scores from uploaded leaf images.

---

## 🧠 Deep Learning Models Used

The following pre-trained CNN architectures were used:

| Model              | Description                                                                             |
| ------------------ | --------------------------------------------------------------------------------------- |
| **ResNet50**       | Uses residual connections to enable training of deeper neural networks efficiently.     |
| **EfficientNetB0** | Provides an efficient balance between network depth, width, and image resolution.       |
| **DenseNet121**    | Uses dense connections between layers to improve feature reuse and gradient flow.       |
| **MobileNetV2**    | A lightweight CNN architecture suitable for efficient and mobile-friendly applications. |

These models were fine-tuned using **Transfer Learning** for mango leaf disease classification.

---

## ⚙️ Technologies Used

* **Python**
* **TensorFlow**
* **Keras**
* **Streamlit**
* **NumPy**
* **Pandas**
* **Matplotlib**
* **Plotly**
* **Pillow (PIL)**
* **Scikit-learn**

---

## 📂 Project Structure

```text
Mango-Leaf-Disease-Detection/
│
├── app.py
│
├── models/
│   ├── ResNet50.keras
│   ├── EfficientNetB0.keras
│   ├── DenseNet121.keras
│   └── MobileNetV2.keras
│
├── dataset/
│   ├── train/
│   ├── validation/
│   └── test/
│
├── notebooks/
│   └── Mango_Leaf_Disease_Training.ipynb
│
├── assets/
│   └── images/
│
├── requirements.txt
│
└── README.md
```

> **Note:** Modify the folder structure above according to your actual GitHub repository.

---

## 🔄 Project Workflow

The overall workflow of the project is:

```text
Mango Leaf Image
       │
       ▼
Image Upload
       │
       ▼
Image Preprocessing
       │
       ▼
Selected Deep Learning Model
       │
       ├── ResNet50
       ├── EfficientNetB0
       ├── DenseNet121
       └── MobileNetV2
       │
       ▼
Disease Classification
       │
       ▼
Prediction + Confidence Score
```

---

## 🖼️ Image Preprocessing

The input mango leaf images undergo preprocessing before being passed to the Deep Learning models.

The preprocessing pipeline includes:

* Image resizing to the required input dimensions.
* Conversion of images into numerical arrays.
* Normalization/scaling of pixel values.
* Reshaping the image to match the model input format.
* Data augmentation during training to improve model generalization.

Typical data augmentation techniques include:

* Rotation
* Horizontal flipping
* Zooming
* Width and height shifting
* Other transformations to improve robustness

---

## 🚀 Streamlit Web Application

The project includes an interactive web application built using **Streamlit**.

### Main Features

* 📤 Upload mango leaf images.
* 🤖 Select from multiple trained Deep Learning models.
* 🔍 Predict the disease category.
* 📊 Display prediction confidence.
* 📈 Visualize model confidence using interactive charts.
* ⚖️ Compare the performance of different models.
* 🌱 Display information related to the predicted disease.

### Application Workflow

1. Select a Deep Learning model.
2. Upload an image of a mango leaf.
3. The image is preprocessed automatically.
4. The selected model analyzes the image.
5. The predicted class is displayed.
6. The prediction confidence is shown using a visualization.

---

## 💻 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/mango-leaf-disease-detection.git
```

### 2. Navigate to the Project Directory

```bash
cd mango-leaf-disease-detection
```

### 3. Install Required Libraries

```bash
pip install -r requirements.txt
```

### 4. Run the Streamlit Application

```bash
streamlit run app.py
```

The application will open in your browser.

---

## 📦 Requirements

Create a `requirements.txt` file containing:

```text
streamlit
tensorflow
numpy
pandas
matplotlib
plotly
Pillow
scikit-learn
```

Install all dependencies using:

```bash
pip install -r requirements.txt
```

---

## 📊 Model Evaluation

The Deep Learning models can be evaluated using the following metrics:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix
* Training Accuracy
* Validation Accuracy
* Training Loss
* Validation Loss

The models are compared to determine which architecture performs best on the mango leaf disease dataset.

---

## 📈 Performance Comparison

A comparison of the implemented models can be added below after training:

| Model          | Test Accuracy | Precision | Recall | F1 Score |
| -------------- | ------------: | --------: | -----: | -------: |
| ResNet50       |           XX% |       XX% |    XX% |      XX% |
| EfficientNetB0 |           XX% |       XX% |    XX% |      XX% |
| DenseNet121    |           XX% |       XX% |    XX% |      XX% |
| MobileNetV2    |           XX% |       XX% |    XX% |      XX% |

> Replace `XX%` with your actual experimental results.

---

## 🌟 Key Features

* Uses **Transfer Learning** for improved classification performance.
* Compares multiple state-of-the-art CNN architectures.
* Supports real-time image prediction.
* Displays prediction confidence.
* Interactive and user-friendly Streamlit interface.
* Can be extended for deployment in agricultural monitoring systems.
* Potential application in **smart farming and precision agriculture**.

---

## 🔮 Future Improvements

Future versions of this project can include:

* Integration of additional Deep Learning architectures.
* Larger and more diverse mango leaf datasets.
* Disease severity estimation.
* Real-time detection using a mobile camera.
* Deployment on cloud platforms.
* Development of an Android or iOS application.
* Integration with IoT-based smart agriculture systems.
* Multilingual support for farmers.
* Recommendation of possible preventive measures based on the detected disease.

---

## 🌍 Real-World Applications

This system can potentially be used in:

* 🌱 Smart Agriculture
* 🥭 Mango Farms and Orchards
* 📱 Mobile-Based Plant Disease Detection
* 🚜 Precision Farming
* 🤖 AI-Based Agricultural Monitoring Systems

---

## 🎓 Learning Outcomes

Through this project, the following concepts were explored:

* Deep Learning
* Convolutional Neural Networks
* Transfer Learning
* Image Classification
* Data Augmentation
* Model Evaluation
* Computer Vision
* Streamlit Web Development
* Deployment of Machine Learning Models

---

## 🛠️ How the Prediction Works

```text
User uploads mango leaf image
            ↓
Image is resized and preprocessed
            ↓
Selected CNN model processes the image
            ↓
Model generates probabilities for all classes
            ↓
Class with highest probability is selected
            ↓
Predicted disease + confidence score displayed
```

---

## 👨‍💻 Author

**Ashmin Singh**

B.Tech – Electronics and Communication Engineering (ECE)
Bharati Vidyapeeth's College of Engineering, New Delhi

### Connect with Me

* LinkedIn: Add your LinkedIn profile link here
* GitHub: Add your GitHub profile link here

---

## ⭐ Acknowledgements

This project was developed as part of an academic exploration of **Artificial Intelligence, Deep Learning, and Computer Vision**.

Special thanks to the open-source community and the developers of:

* TensorFlow
* Keras
* Streamlit
* Scikit-learn
* Plotly

---

## 📄 License

This project is intended for **educational and research purposes**.

---

### ⭐ If you found this project useful, consider giving the repository a star!

