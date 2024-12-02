# AAI521-Hand-Gestures

Each gesture (G1–G10) is performed by 14 participants (P1–P14) with 10 repetitions.

---

## **Model Architecture**
The model consists of two branches:
1. **Image Branch:**
   - Processes RGB, depth, and raw depth data using convolutional layers.
   - Extracts spatial features for gesture classification.

2. **Leap Motion Branch:**
   - Processes motion features with LSTM layers to capture temporal dependencies.

The two branches are concatenated and passed through dense layers with dropout for regularization. The final output is a softmax activation layer for classification.

---

## **Setup and Installation**
### **Dependencies**
- Python 3.8+
- TensorFlow 2.0+
- OpenCV
- Scikit-learn
- Matplotlib
- NumPy
- Pandas