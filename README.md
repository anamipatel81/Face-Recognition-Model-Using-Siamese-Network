# Face-Recognition-Model-Using-Siamese-Network

A **face recognition system** built with a **Siamese Neural Network** (TensorFlow/Keras), packaged in a **Kivy** app for user-friendly deployment.  

The Siamese Network learns to distinguish between images of the same person and different people by comparing embeddings of face images.

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

## 📂 Project Structure:

    ```bash
    project/
      │
      ├── data/
      │   ├── anchor/         # Anchor face images
      │   ├── positive/       # Positive pairs (same person)
      │   └── negative/       # Negative pairs (different people)
        │
      ├── model/
      │   ├── siamese_model.h5  # Saved trained model
      │   └── embedding_model.h5
      │
      ├── app/
      │   ├── main.py         # Kivy app entry point
      │   ├── screens.kv      # Kivy UI
      │   └── assets/         # App images/icons
      │
      ├── train.py            # Siamese network training script
      ├── verify.py           # Image verification script
      ├── requirements.txt
      └── README.md

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
