# **License Plate Detection and Recognition System**

This project implements a **two-stage AI pipeline** to detect and recognize Iranian license plates using **YOLO (You Only Look Once)** for object detection and **Convolutional Neural Networks (CNNs)** for character recognition.

---

## **Overview**

This project includes:

- **License Plate Detection (LPD)**: Localizing plates in images using YOLOv12.
- **License Plate Recognition (LPR)**: Identifying alphanumeric characters using CNNs.

---

## **Technologies & Libraries**

- Python
- [Ultralytics YOLOv12](https://github.com/ultralytics/ultralytics)
- OpenCV
- Matplotlib
- PyYAML

---

## **Dataset**

The dataset includes:
- Annotated vehicle images with license plates (for detection)
- Cropped license plates (for character recognition)

[Download Dataset](https://drive.google.com/drive/folders/1StRhbI28MaoiuXqA2rG5vGqKG5K2bMW6?usp=sharing)

---

## **Tasks Breakdown**

### **1. License Plate Detection (LPD)**
- Trained YOLOv12 model on custom data.
- Used Ultralytics API for training & testing.
- Evaluated via confidence scores and visual outputs.

### **2. License Plate Recognition (LPR)**
- Designed CNN model to classify:
  - **7 digits + 1 Persian letter**.
- Trained on cropped plates from LPD output.
- Achieved high character-level accuracy.

### **3. Pipeline Integration**
- YOLO model detects plate region.
- CNN recognizes characters from cropped plate.
- End-to-end license plate number generated.

### **4. Evaluation**
- **Detection**: mAP (mean Average Precision)
- **Recognition**: Character-level accuracy
- Visualized full plate predictions

---

## **Learning Outcomes**

- Applied YOLOv12 for real-world detection
- Developed and trained CNNs for classification
- Integrated models into a seamless end-to-end pipeline
- Evaluated deep learning system performance

---

## **Performance Results**

**The system achieves a character recognition accuracy of 93.87% and an F1-score of 0.94 for license plate detection.**

**Final YOLO Detection Results on Test Set:**

- **mAP@50-95**: 0.75  
- **mAP@50**: 0.97  
- **mAP@75**: 0.87  
- **Precision**: 0.95  
- **Recall**: 0.935

## **Sample Results**

*Add visual examples of predictions here*

---

## **References**

- [YOLOv12 Documentation](https://docs.ultralytics.com/)
- [YOLOv12 Architecture Overview (Video)](https://youtube.com/playlist?list=PL8VDJoEXIjppNvOzocFbRciZBrtSMi81v)
- [Ultralytics Model Docs](https://docs.ultralytics.com/models/)

---

## **Author**

**Amir Vahedi**  
M.Sc. in Computer Engineering – Artificial Intelligence  
Sharif University of Technology

---
