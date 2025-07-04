# Face-Recognition-Model-Using-Siamese-Network

A **face recognition system** built with a **Siamese Neural Network** (TensorFlow/Keras), packaged in a **Kivy** app for user-friendly deployment.  

It can verify whether **two face images belong to the same person**.

---

## 🚀 Features

- Siamese Neural Network for image verification
- CNN-based embedding model
- Easy-to-use Kivy GUI
- Command-line verification option

---

## Installation:

1. Clone the repository:
   ```bash
   git clone https://github.com/anamipatel81/Face-Recognition_model-Using-Siamese-Network.git
   cd Face-Recognition_model-Using-Siamese-Network
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt

---

## Project Structure:

face-recognition/<br>
│<br>
├── data/<br>
│ ├── anchor/ # Anchor images<br>
│ ├── positive/ # Positive pairs (same person)<br>
│ └── negative/ # Negative pairs (different people)<br>
│<br>
├── model/<br>
| ├── embedding<br>
| ├── L1.Dist<br>
│ ├── siamese_model<br>
│<br>
├── app/<br>
  ├── application_data<br>
    ├── input_image<br>
    ├── verification_image<br>
  ├── siamesemodelv2.h5<br>
  ├── layers.ky # Contain custom L1Dist Layer<br>
  └── faceid.py # Main script for recognition app<br>

---

## 📈 Model Details:

1. Embedding Model:
CNN for feature extraction

2. Distance Layer:
Computes absolute difference

3. Classifier:
Single sigmoid unit for match probability

## Future Improvement:

- Improve training data size and quality
- Perform Data Augmentation for better result
- Optimized model conversion (e.g. TensorFlow Lite)
  
## 🙏 Acknowledgements:
- Siamese Neural Networks for One-shot Image Recognition (Research Paper)
- Kivy community documentation
