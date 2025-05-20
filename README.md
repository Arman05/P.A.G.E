# 👤 Person Detection and Gender, Age, and Ethnicity Classification System

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
![Simulation Running](https://github.com/Arman05/P.A.G.E/blob/main/Crowd%20Image%20Sample.png) 
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

```

## 🖼️ Usage
Run the detection and classification on an image:

python detect_and_classify.py --image path/to/image.jpg

## ⚙️ Command-Line Options

| Argument    | Description                                                     |
| ----------- | --------------------------------------------------------------- |
| `--image`   | Path to the input image                                         |
| `--output`  | (Optional) Path to save the output image                        |
| `--display` | Whether to display the image in a pop-up window (default: True) |
| `--conf`    | Detection confidence threshold (default: `0.5`)                 |

## Example
python detect_and_classify.py --image input.jpg --output result.jpg --conf 0.6

## 💼 Use Cases

  * 🏪 Retail: Count and profile visitors for better service
  * 🏨 Hospitality: Understand guest demographics for targeting
  * 🏙️ Urban Planning: Analyze pedestrian trends at crossings or events
  * 🎥 Security: Use demographic detection for video surveillance
  * 📊 Business Intelligence: Generate real-time demographic statistics


## 🙏 Acknowledgements

 * [Faster R-CNN Paper](https://arxiv.org/abs/1506.01497)
 * [COCO Dataset](https://cocodataset.org/#home)
 * [PASCAL VOC Dataset](http://host.robots.ox.ac.uk/pascal/VOC/)
 * [UTKFace Dataset](https://susanqq.github.io/UTKFace/)
 * [FairFace Dataset](https://github.com/joojs/fairface)



## 📄 License

  This project is licensed under the MIT License. See the LICENSE file for more details.
