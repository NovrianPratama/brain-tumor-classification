# 🧠 Brain Tumor Classification using MRI Images

This project focuses on classifying brain tumors using MRI images into four categories using deep learning. The aim is to support early detection of brain tumors, which plays a vital role in determining effective treatment and improving patient outcomes.

---

## 📚 About the Dataset

The dataset used is from Kaggle: **Brain Tumor MRI Dataset**, which is a combination of:

- **Figshare**
- **SARTAJ Dataset** _(some glioma images were removed due to mislabeling)_
- **Br35H**

### Dataset Details:

- 📷 **Total Images**: 7023
- 🧠 **Classes**:
  - Glioma
  - Meningioma
  - Pituitary
  - No Tumor (from Br35H)

⚠️ _Note: The original image sizes vary. As part of preprocessing, all images were resized and unnecessary margins were removed to improve model performance._

---

## 🧪 Methods

This project uses a **Convolutional Neural Network (CNN)** architecture to:

- Detect and classify brain tumors
- Train a single model capable of handling multiple classification tasks
- Prepare the trained model for multiple deployment environments (TF, TFLite, TFJS)

The entire training and evaluation process is documented in the `notebook.ipynb`.

---

## 🗂 Project Structure

brain-tumor-classification/
├── models/
│ ├── saved_model/ # SavedModel format
│ ├── tflite/ # TensorFlow Lite model
│ └── tfjs/ # TensorFlow.js model
├── data/
│ ├── Training/ # Training images
│ └── Testing/ # Testing images
├── brain_tumor_classification.ipynb # Main notebook
├── requirements.txt # Dependencies
└── README.md # This files
