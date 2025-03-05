# EmotionLens: AI-Powered Facial Expression Recognition System

## Overview

**EmotionLens** is an AI-based facial expression recognition system that employs a **custom Convolutional Neural Network (CNN)** to classify human emotions accurately. The project is designed to enhance emotion analysis, mental health monitoring, and human-computer interaction by providing a reliable and scalable emotion detection model.

### Problem Statement

Facial expression recognition (FER) is crucial for various applications, including behavioral studies, security, and emotional AI. However, existing models face challenges such as:
- **Subtle Expression Differentiation:** Difficulty in distinguishing similar emotions like fear and surprise.
- **Environmental Variability:** Sensitivity to lighting conditions, facial pose variations, and occlusions.
- **Limited Generalization:** Many models perform well on specific datasets but fail in diverse real-world conditions.

To address these issues, EmotionLens is built with a custom CNN architecture, eliminating dependencies on pre-trained models and ensuring better adaptability and efficiency.

## Contributors

👨‍💻 **Manvendra Singh** - [LinkedIn](#) | [GitHub](#)  
👨‍💻 **Kshitiz Bhargava** - [LinkedIn](#) | [GitHub](#)  

**Affiliation:** Department of Software Systems, School of Computer Science & Engineering, Vellore Institute of Technology, India.  

## Features & Highlights

- **Custom CNN Model:** Tailored for facial expression recognition with optimized feature extraction layers.
- **Emotion Classification:** Detects eight emotions - **Surprise, Fear, Neutral, Sad, Disgust, Contempt, Happy, and Anger**.
- **Real-time Recognition:** Supports image uploads for instant emotion prediction.
- **Optimized Performance:** Eliminates reliance on pre-trained models, ensuring efficiency and interpretability.
- **Scalability:** Future-ready to accommodate additional emotion categories and real-world datasets.

## Dataset

EmotionLens is trained on **28,175 images**, covering the following emotions:
- Surprise (~16.4%)
- Happy (~15.4%)
- Neutral (~10.2%)
- Sad (~10.6%)
- Fear, Disgust, Contempt, and Anger (~11-13% each)

The dataset is balanced to minimize bias, ensuring robust model performance across all emotion categories.

## Model Architecture

The **EmotionLens CNN model** comprises:
1. **Convolutional Layers:** Extract hierarchical features from facial images.
2. **Batch Normalization & Dropout:** Enhances training stability and prevents overfitting.
3. **Activation Functions:** Uses ReLU and Softmax for non-linearity and classification.
4. **Optimization:** Trained with Adam optimizer and cross-entropy loss for efficient learning.

## Results & Evaluation

EmotionLens achieves high classification performance:
- **F1 Score:** 0.7425
- **Multiclass ROC AUC Score:** 0.9642

## Running the Model

### 1. Clone the Repository
```sh
 git clone https://github.com/yourusername/EmotionLens.git
 cd EmotionLens
```

### 2. Install Dependencies
```sh
pip install -r requirements.txt
```

### 3. Run the Model
```sh
python EmotionLens.py
```

### 4. Test with an Image
Upload an image to test the emotion detection:
```sh
python test_image.py --image sample.jpg
```

## Acknowledgments

Special thanks to **Prof. Krishnaraj N** for guidance and support throughout this research. We also appreciate the contributions from the **VIT research community** and the open-source developers who provided essential tools and frameworks.

## License

This project is intended for academic and research use only. For commercial usage, please seek permission from the authors.

---

