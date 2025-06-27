# DEEP_LEARNING_PROJECT

COMPANY: CODTECH IT SOLUTIONS

NAME: PARTH CHANDWANI

INTERN ID: CT08DF409

DOMAIN: DATA SCIENCE

DURATION: 8 WEEKS

MENTOR: NEELA SANTOSH

DESCRIPTION OF THE TASK:

---

# 🧠 CIFAR-10 Image Classification using CNN in PyTorch

## 📌 Overview

This project implements a Convolutional Neural Network (CNN) using **PyTorch** to classify images from the **CIFAR-10 dataset**, which includes 10 object categories such as airplane, car, bird, cat, deer, dog, frog, horse, ship, and truck.

The script handles:

* Data preprocessing
* CNN model definition
* Training and validation loop
* Accuracy calculation
* Visualization of predictions
* Performance plots

---

## 📂 Files

| File Name                 | Description                                                |
| ------------------------- | ---------------------------------------------------------- |
| `image_classification.py` | Main script containing the CNN model and training pipeline |
| `Figure_1.png`            | Sample training images preview                             |
| `Figure_2.png`            | True vs predicted labels visualization                     |
| `Graph_1.png`             | Training and validation accuracy/loss curves               |

---

## 📊 Dataset: CIFAR-10

* **Training Samples**: 50,000
* **Test Samples**: 10,000
* **Classes**:

  ```
  ['plane', 'car', 'bird', 'cat', 'deer', 
   'dog', 'frog', 'horse', 'ship', 'truck']
  ```

---

## 🧱 Model Architecture

A basic CNN model with the following structure:

```
Conv2D(3, 6, 5) → ReLU → MaxPool2D
Conv2D(6, 16, 5) → ReLU → MaxPool2D
Flatten
Linear(16*5*5 → 120) → ReLU
Linear(120 → 84) → ReLU
Linear(84 → 10) → Output Classes
```

---

## 🧪 Training Details

* **Loss Function**: CrossEntropyLoss
* **Optimizer**: SGD with Momentum (0.9)
* **Epochs**: 10
* **Batch Size**: 4
* **Device**: CPU/GPU (automatic detection)

---

## 📉 Performance Graphs

### Training & Validation Loss and Accuracy

📎 *`Graph_1.png`*
Shows convergence and overfitting trends.

* **Training Loss** steadily decreases.
* **Validation Accuracy** peaks around 62%, indicating the model is generalizing fairly.

---

## 🎯 Accuracy

* **Overall Test Accuracy**: \~62%
* **Per-Class Accuracy** is also printed in the terminal, showing how well the model performs per label.

---

## 🖼️ Visual Outputs

### 1. Training Images

📎 *`Figure_1.png`*
Displays a grid of random training images with their labels.

### 2. Prediction Visualization

📎 *`Figure_2.png`*
Each image is annotated with:

* ✅ `True:` ground truth label (green)
* ❌ `Pred:` predicted label (red if incorrect)

---

## 🚀 How to Run

1. Install PyTorch:

   ```bash
   pip install torch torchvision matplotlib
   ```

2. Run the script:

   ```bash
   python image_classification.py
   ```

3. Output graphs and prediction visuals will appear automatically.

---

## 📈 Example Output Snippet

```
Epoch 10, 
Train Loss: 0.86, Train Acc: 70.0%, 
Validation Loss: 1.18, Validation Acc: 62.0%

Accuracy of the network on the 10000 test images: 62%
Accuracy of frog  : 72.34 %
Accuracy of car   : 71.12 %
...
```

---

## 📌 Notes

* The training is basic and could be improved with:

  * More epochs
  * Data augmentation
  * Dropout / BatchNorm
  * Better architecture (ResNet, etc.)

![Image](https://github.com/user-attachments/assets/858cf22b-316f-4e7c-ace3-5dcb310f3ed7)
![Image](https://github.com/user-attachments/assets/ac1051b0-4e33-4a41-a440-d294ea814672)
![Image](https://github.com/user-attachments/assets/278150a5-c37d-4ce2-98fc-036c96946fcc)
![Image](https://github.com/user-attachments/assets/cc643282-4e1f-45cd-9846-4a252725d27c)
![Image](https://github.com/user-attachments/assets/a8e0baaa-5ebd-43f7-a1e2-6a8d4238dd17)
