# AI-Powered Yoga Pose Detection and Evaluation System (PoseNet + VGG16)

## Overview
This repository contains the code and resources for an **AI-Powered Yoga Pose Detection and Evaluation System** developed as a **final-year undergraduate capstone project**. The system uses a **hybrid deep-learning approach combining PoseNet and VGG16** to **classify yoga poses from images/webcam frames** and **validate** whether the detected pose matches a target pose. The output includes the predicted pose label (e.g., *Goddess*) along with a confidence score and a **Valid/Invalid** indicator.

This project was later converted into a research paper and resulted in an **Indian patent application** (published in the Indian Patent Journal).

---

## Project Highlights
- Yoga pose classification using deep learning
- Pose validation (Valid/Invalid) based on target pose matching
- Two model variants:
  - **Proposed VGG16** (image-only classifier baseline)
  - **Proposed PoseNet** (Proposed VGG16 fused with Proposed PoseNet - hybrid approach using keypoints + visual features)

---

## Repository Contents
- **Proposed_VGG16.ipynb**  
  Baseline VGG16 transfer learning model for yoga pose classification.

- **Proposed_PoseNet_Combined_with_VGG16.ipynb**  
  Hybrid notebook using PoseNet keypoints (TensorFlow Hub) combined with VGG16 for pose classification + validation.

---

## Features
- **Pose Classification:** Predicts the yoga pose label from an input image/frame
- **Pose Validation:** Verifies if the predicted pose matches the selected target class
- **Confidence Score:** Outputs model confidence for the prediction
- **Notebook-based Workflow:** Training, inference, and evaluation are provided in Jupyter notebooks

---

## Tech Stack
- **Programming:** Python
- **Deep Learning:** TensorFlow, Keras
- **Pose Estimation:** TensorFlow Hub (PoseNet)
- **Computer Vision:** OpenCV, Pillow
- **Data & Visualization:** NumPy, Pandas, Matplotlib, Seaborn

---

## Dataset Setup
The VGG16 notebook expects a dataset organized by class.

Example structure:


In the original notebooks, the dataset path was used via Google Drive (Colab):
- `/content/drive/My Drive/Yoga/DATASET/TRAIN`
- `/content/drive/My Drive/Yoga/DATASET/TEST`

If running locally, update paths inside the notebooks to match your dataset location.

---

## Getting Started

### Have run code in Google Colab
1. Upload notebooks to Colab or open them from GitHub.
2. Mount Google Drive:
```python
from google.colab import drive
drive.mount('/content/drive')

3. Ensure your dataset/model paths match your Drive structure (update paths in the notebook if needed).

4. Run the notebook cells in order:
    - Run Proposed_VGG16.ipynb for training + evaluation
    - Run Proposed_PoseNet.ipynb for hybrid inference + validation

---

## Output Example

**Final Prediction: Goddess (Valid, 98.33%)**

**Meaning:**
- **Pose predicted:** Goddess  
- **Validation:** Valid (matches target pose)  
- **Confidence:** 98.33%  

---

## Patent / Publication

**Indian Patent Application No.: 202541122968 — Published in Indian Patent Journal (U/S 11A).**





