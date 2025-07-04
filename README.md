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
      |
      ├── model/
      |   ├── emmending       # CNN 
      │   ├── L1Dist Layer    # Compute L1 Distance (absolute difference) 
      │   └── siamese_model
      │
      ├── app/
          ├── application_data
              ├── input_image
              └── verification_image
          ├── siamesemodelv2.h5 # Saved trained model
          ├── layers.py         # Contain custom L1Dist Layer
          └── faceid.py         # Main scripy for face recognition app

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
