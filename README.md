# EtechCycle NTHS Hackathon
Here’s your updated README with the project name changed to:

# ♻️ EtechCycle – AI-Powered E-Waste Detection System

EtechCycle is an AI-driven computer vision project built using YOLOv8 to detect and classify electronic waste in real-time. The system uses a custom-trained deep learning model to identify e-waste objects through a webcam feed, helping promote proper recycling and sustainable waste management.

Instead of manually sorting electronic waste, EtechCycle provides automated, intelligent detection powered by modern AI/ML technologies.

---

## 🚀 Features

🔍 **Real-Time Detection** – Detects e-waste objects live using webcam input.

🧠 **Custom YOLOv8 Model** – Trained on a specialized e-waste dataset for accurate classification.

⚡ **GPU Acceleration** – Utilizes CUDA when available for faster training and inference.

🎥 **Live Computer Vision Pipeline** – OpenCV integration for real-time frame processing and visualization.

📊 **Model Training Pipeline** – Fully configurable YOLOv8 training setup.

---

## 🛠️ Tech Stack

**AI Framework:** Ultralytics YOLOv8
**Deep Learning:** PyTorch
**Computer Vision:** OpenCV
**Language:** Python
**Hardware Acceleration:** CUDA (if available)

---

## 📂 Project Structure

```
EtechCycle/
│── main.py                  # Real-time detection script
│── train.py                 # Model training script
│── e_waste_dataset/
│     └── data.yaml          # Dataset configuration
│── runs/                    # Training outputs
│── train_e_waste_fixed11/
│     └── weights/
│          └── best.pt       # Best trained model weights
```

---

## 🔑 Setup Instructions

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/EtechCycle.git
cd EtechCycle
```

---

### 2️⃣ Install Dependencies

```bash
pip install ultralytics opencv-python torch
```

Or using a requirements file:

```bash
pip install -r requirements.txt
```

---

### 3️⃣ Train the Model

```bash
python train.py
```

Training Configuration:

* Epochs: 50
* Image Size: 640
* Batch Size: 8
* Mixed Precision (AMP): Enabled
* Device: CUDA (if available)

---

### 4️⃣ Run Real-Time Detection

```bash
python main.py
```

Press **Q** to exit the live detection window.

---

## 🧠 How It Works

1. The model initializes with YOLOv8 nano (`yolov8n.pt`) as a pretrained base.
2. The custom e-waste dataset fine-tunes the model.
3. The best weights (`best.pt`) are saved after training.
4. Webcam frames are passed into the trained model.
5. Detected objects are annotated and displayed in real-time.

---

## 🎯 Roadmap

* Improve dataset size and diversity for higher accuracy.
* Deploy as a web-based application.
* Add recycling category recommendations.
* Integrate analytics dashboard for detection insights.
* Optimize for edge deployment (Raspberry Pi / Jetson).

---

## 🌍 Problem Statement

Electronic waste is one of the fastest-growing waste streams globally. Improper disposal leads to environmental pollution and serious health hazards.

EtechCycle aims to:

* Automate identification of electronic waste
* Assist recycling facilities in smart sorting
* Promote sustainable environmental practices

---

## 👥 Team

* Kevin Bheemarasetti
* Joel Joseph
* Aditi Sharma
* Vivek Vardhan Sai Sirigirisetty

---

## 🙌 Acknowledgments

This project was a collaborative effort focused on solving real-world environmental challenges using AI/ML technologies.

Working through dataset preparation, GPU configuration, model optimization, and real-time inference strengthened our understanding of computer vision systems and deep learning workflows.

EtechCycle provided hands-on experience in:

* Custom object detection training
* Model fine-tuning
* Real-time deployment pipelines
* AI-driven sustainability solutions

We look forward to expanding this into a scalable environmental AI system. ♻️🚀

---

