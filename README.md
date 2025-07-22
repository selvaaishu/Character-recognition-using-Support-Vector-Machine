Character Recognition using Support Vector Machine (SVM)

This project demonstrates how to build a character recognition model using the Support Vector Machine (SVM) algorithm with the load_digits dataset available in scikit-learn. The goal is to recognize handwritten digits (0–9).


---

📚 Dataset

We use the load_digits() dataset from sklearn.datasets, which consists of 1,797 8x8 images of handwritten digits.

Total Samples: 1797

Image Size: 8x8 (64 features)

Classes: 10 (Digits 0 to 9)



---

🛠 Tools & Libraries Used

Python 🐍

scikit-learn 🤖

NumPy 🔢

Matplotlib 📊



---

📦 Installation

Make sure you have the following packages installed:

pip install numpy matplotlib scikit-learn


---

🚀 How to Run

1. Clone the repository or copy the code file.


2. Run the Python script:



python character_recognition_svm.py


---

🧠 Model Overview

We use the Support Vector Classifier (SVC) from sklearn.svm:

from sklearn.svm import SVC
model = SVC(kernel='linear', gamma=0.001)


---

📈 Evaluation

We split the dataset using train_test_split.

Evaluate using classification_report and accuracy_score.



---

📊 Sample Output

Accuracy: 0.97

Classification Report:
              precision    recall  f1-score   support

           0       1.00      1.00      1.00        45
           1       0.95      1.00      0.98        45
           ...
           9       0.96      0.92      0.94        39


---

🔍 Visualization

Plot a few predicted images alongside actual labels for visual comparison.

plt.imshow(digits.images[0], cmap=plt.cm.gray_r)
plt.title(f"Prediction: {prediction[0]}")
