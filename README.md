# 👤 Person Detection and Demographic Classification with FRCNN

This project implements two fundamental computer vision tasks:

1. **Person Detection** – Identifying and localizing people within an image using bounding boxes.
2. **Demographic Classification** – Predicting the **age**, **race**, and **gender** of each detected individual.

Built with **Faster R-CNN (FRCNN)** from the R-CNN model family, the system is capable of detecting people from various angles, poses, and levels of obstruction. Once detected, demographic attributes are classified using dedicated models trained on diverse datasets.

---

## 🚀 Features

- 📦 Person detection with bounding boxes
- 🔍 Age, gender, and race classification
- 🎯 Works even when persons are not the main subject
- 🎥 Supports image input and adaptable to video streams
- 💪 Handles multiple poses and partial occlusion

---

## 📚 Datasets

This project leverages multiple public datasets for both detection and classification tasks:

### 👤 Person Detection:
- [PASCAL VOC](http://host.robots.ox.ac.uk/pascal/VOC/)
- [COCO (Common Objects in Context)](https://cocodataset.org/)

### 🧬 Demographic Classification:
- [UTKFace](https://susanqq.github.io/UTKFace/)
- [FairFace](https://github.com/joojs/fairface)

---

## 🛠️ Installation

Clone the repository and install the necessary dependencies:

```bash
git clone https://github.com/your-username/person-detection-demographics.git
cd person-detection-demographics

# (Optional) Create a virtual environment
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

