# AquaGuard: AI-Powered Underwater Pollution Detection and Classification

**Authors**:  
- Sıla Keskin ([damlasilakeskin@gmail.com](mailto:damlasilakeskin@gmail.com))  
- Kağan Canerik ([kagancanerik@gmail.com](mailto:kagancanerik@gmail.com))  
- Tuğba Gürgen Erdoğan ([tugba@cs.hacettepe.edu.tr](mailto:tugba@cs.hacettepe.edu.tr))  

**Institution**:  
Hacettepe University, Computer Engineering Department, Software Engineering Research Group, Ankara, Turkey  

---

## 📖 Project Overview

AquaGuard is a machine learning-based system designed to monitor and classify underwater pollution. By leveraging the YOLOv8 object detection model and a custom pollution risk scoring algorithm, the system categorizes underwater scenes into three risk levels:  
- **Low pollution risk**  
- **Medium pollution risk**  
- **High pollution risk**  

This innovative approach aims to enhance marine environmental monitoring, providing a scalable and automated solution to assess pollution severity in real time.

---

## 🚀 Features

- **Object Detection**: Detects debris such as plastics, metals, and fishing nets using YOLOv8.  
- **Pollution Scoring**: Assigns pollution coefficients to objects to calculate a risk score for each image.  
- **Classification**: Categorizes underwater scenes into pollution severity levels (Low, Medium, High).  
- **Data Augmentation**: Improved classification accuracy through data augmentation techniques.  

---

## 🔧 Methodology

### **Dataset**  
- **Source**: [Underwater Plastic Pollution Dataset](https://www.kaggle.com/datasets/arnavs19/underwater-plastic-pollution-detection/data)  
- **Structure**:
  - **Train**: 3,628 images  
  - **Validation**: 1,001 images  
  - **Test**: 501 images  
- **Enhancements**: Images preprocessed using the Dark Prior Channel method to improve underwater object visibility.

### **Object Detection**  
- **Model**: YOLOv8  
- **Pretrained Weights**: YOLOv8 fine-tuned on the underwater pollution dataset.

### **Classification**  
- A custom pollution scoring algorithm assigns weights to detected objects.  
- Scores are aggregated and used to classify images into pollution risk levels.

---

## 📊 Results

### **Without Data Augmentation**
- **Risk Level Classification Accuracy**: 79%  
- **Object Detection Accuracy**: 86%  

### **With Data Augmentation**
- **Risk Level Classification Accuracy**: 85%  
- **Object Detection Accuracy**: 92%  

---

## 🛠️ Installation & Usage

### Prerequisites
- Python 3.8+
- Required Libraries:
  ```bash
  pip install requirements.txt

Training and testing parts are placed on underwater.ipynb file
For privacy reasons, we cannot add api code, you can contact us for dataset.
:)
