# <img src="https://github.com/manvendrasingh09/EmotionLens/blob/main/Resources/EmotionLens.jpeg" alt="EmotionLens Logo" width="30" style="vertical-align: middle;"/> EmotionLens: Optimizing FER with a Lightweight Residual CNN Architecture

## Overview

This repository presents the research titled **"Optimizing Facial Expression Recognition (FER) with a Lightweight Residual CNN Architecture"**, conducted at **Vellore Institute of Technology (VIT), India**.

The project, **EmotionLens**, introduces a novel AI-powered facial expression recognition system leveraging **Residual Convolutional Neural Networks (ResNet CNNs)** to enhance emotion classification accuracy and real-time performance. This repository outlines the methodology, datasets, and results.

---

## Contributors

👨‍💻 **Manvendra Singh** - [Linkedin](https://www.linkedin.com/in/manvendrasingh09) | [Github](https://github.com/manvendrasingh09)

👨‍💻 **Kshitiz Bhargava** - [Linkedin](https://www.linkedin.com/in/kshitiz-bhargava) | [Github](https://github.com/Kshitiz-b)

> **Affiliation:** Department of Software Systems, School of Computer Science & Engineering, Vellore Institute of Technology, India.  
> **Contact Emails:** m.s.jaunpur@gmail.com, kshitizb168@gmail.com

---

## Project Highlights

- **Problem Addressed:** Despite advancements, FER models struggle with real-world generalization due to subtle expression variations, environmental conditions, and dataset limitations. Existing pre-trained models are computationally expensive and not optimized for FER-specific tasks.
- **Solution Provided:** EmotionLens utilizes a deep learning approach featuring:
  - **Custom Residual CNN Architecture** - Optimized for subtle expression recognition using hierarchical feature extraction.
  - **Regularization Techniques** - Implementing batch normalization, dropout, and LeakyReLU activation to improve training stability and prevent overfitting.
  - **Data Augmentation** - Image preprocessing, resizing, and augmentation techniques to enhance model generalization across various facial expressions.
- **Key Achievement:** EmotionLens achieves high accuracy, precision, and recall, outperforming conventional FER models by improving interpretability and computational efficiency.

---

## Methodology

### Proposed Architecture
The **EmotionLens** model integrates:

1. **Residual Convolutional Neural Network (ResNet CNN):**
   - Designed specifically for FER to improve gradient propagation and feature specificity.
   - Includes LeakyReLU activation, batch normalization, and dropout layers for optimized learning.
   
2. **Dataset Augmentation:**
   - Image resizing, normalization, and brightness adjustments to improve robustness.
   - Augmentation techniques such as rotation, flipping, and scaling to enhance model adaptability across diverse expressions.

<img src="https://github.com/manvendrasingh09/EmotionLens/blob/main/Resources/Architecture.png"/>

### Dataset

EmotionLens is trained on the **AffectNet dataset**, consisting of **28,175 high-resolution images**, categorized into eight emotions:

| Emotion  | Percentage |
|----------|-----------|
| Surprise | ~16.4%    |
| Happy    | ~15.4%    |
| Neutral  | ~10.2%    |
| Sad      | ~10.6%    |
| Fear, Disgust, Contempt, Anger | ~11-13% each |

The dataset is **balanced**, ensuring fair representation across all emotion classes.

<img src="https://github.com/manvendrasingh09/EmotionLens/blob/main/Resources/Dataset.png" width="500"/>

---

## Results

### Model Performance
| Metric                | Value  |
|----------------------|--------|
| **Test Accuracy**   | 73.96% |
| **F1 Score**       | 0.7426  |
| **Multiclass ROC AUC Score** | 0.9643 |

### Evaluation Metrics
- **Confusion Matrix:**
  - Analyzes correct and misclassified expressions across emotion categories.

<img src="https://github.com/manvendrasingh09/EmotionLens/blob/main/Resources/Confusion%20Matrix.png" width="500"/>
  
- **ROC-AUC Curve:**
  - A mean AUC score of **0.96+** confirms high confidence in model predictions.

<img src="https://github.com/manvendrasingh09/EmotionLens/blob/main/Resources/ROC.png" width="500"/>

- **Comparative Performance:**
  - Outperforms traditional FER models like VGG-Face, Norface, and Multi-task EfficientNet-B2 on the AffectNet dataset. [Source](https://paperswithcode.com/sota/facial-expression-recognition-on-affectnet)
 
<img src="https://github.com/manvendrasingh09/EmotionLens/blob/main/Resources/PwC%20Graph.png" width="500"/>

---

## Run Locally with [Docker](https://hub.docker.com/r/kshitizb/emotionlens)

### **1. Pull the Image**
```sh
docker pull kshitizb/emotionlens
```

### **2. Run the Container**
```sh
docker run -p 8010:8010 kshitizb/emotionlens
```
Then open: **http://localhost:8010/**

### **3. Access the API**
Once the container is running, open a browser and go to:

```
http://<your-server-ip>:8010
```

Or test via **FastAPI interactive docs**:

```
http://<your-server-ip>:8010/docs
```

---

## **Endpoints**
| Method  | Endpoint       | Description |
|---------|---------------|-------------|
| **GET** | `/`           | Homepage - Image Upload Form |
| **POST** | `/upload/`   | Upload and classify an image |

---

## Acknowledgments

We would like to express our sincere gratitude to:
- **VIT University** for providing the platform and resources to conduct this research.
- **Our mentors and advisors** for their continuous guidance and constructive feedback throughout the project.
- **Contributors and researchers** in the field of emotion detection whose work inspired and informed our approach.
- **The open-source community** for providing valuable tools and frameworks that enabled the development of this model.
  
---

## License

This project is released for academic and research purposes only.  
You can view and access the source code from our repository, but any commercial use or distribution requires prior permission.  

🔗 **[EmotionLens Source Code](https://github.com/manvendrasingh09/EmotionLens/blob/main/Resources/EmotionLens.ipynb)**  

For inquiries regarding licensing and usage, please contact the authors.
