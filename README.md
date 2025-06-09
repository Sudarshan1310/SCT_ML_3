# 🐾 SVM Cat vs Dog Image Classifier

This project implements a **Support Vector Machine (SVM)** to classify images of **cats and dogs**. It demonstrates how classical machine learning methods can be applied to image classification tasks with proper preprocessing.

---

## 📌 Project Overview

- 📂 Dataset: Small image dataset of cats and dogs
- 📐 Image Preprocessing: Resize, flatten, normalize
- 🤖 Model: Scikit-learn's `SVC` with linear kernel
- 🎯 Goal: Predict whether an image is a cat or a dog

---

## 📷 Sample Input

- Images resized to **64x64**
- Flattened to 1D array (64 × 64 × 3 = 12288 features)

---

## 🛠️ Tech Stack

| Tool           | Purpose                         |
|----------------|---------------------------------|
| Python         | Programming language            |
| scikit-learn   | SVM model + evaluation          |
| OpenCV         | Image loading and resizing      |
| NumPy          | Data manipulation               |
| Matplotlib     | Visualization                   |
| Jupyter Notebook | Interactive experimentation  |

---

## 🧪 How It Works

1. Load images from `cat/` and `dog/` folders
2. Resize each image to 64×64
3. Flatten the image into a 1D feature vector
4. Label `cat` as 0 and `dog` as 1
5. Split into training and testing sets
6. Train a **linear SVM**
7. Evaluate accuracy and visualize predictions

---

## 🚀 Running the Project

### 1. Clone the Repository

git clone https://github.com/Sudarshan1310/SCT_ML_3.git
cd svm-cat-dog-classifier

### 2. Install dependecies

pip install -r requirements.txt

### 3. Run the notebook

jupyter notebook

### 📊 Sample Output

Accuracy: 0.88
Accuracy may vary depending on dataset size and image quality.

### 💾 Model Saving
You can save the trained model using joblib:

import joblib
joblib.dump(clf, 'svm_cat_dog.pkl')

### 📁 Folder Structure

```svm-cat-dog-classifier/
├── SVM_Cat_Dog_Classifier.ipynb
├── requirements.txt
├── README.md
└── data/
    ├── cat/
    └── dog/
```

### 📌 Notes
This project is for educational/demo purposes and uses a relatively small dataset.

For production-grade models, consider using CNNs (like in TensorFlow or PyTorch).

### 🧑‍💻 Author
SkillCraft Technology Assignment
Implemented by: G S G Sudarshan

### 📄 License
This project is open source under the MIT License.
