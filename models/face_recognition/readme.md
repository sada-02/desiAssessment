# Face Recognition Setup and Usage Guide

Follow these steps to set up and run the face recognition system:

First run: 
```bash
pip install -r requirements.txt
```

## 1. Download Model Weights

Download the model weights from the following link:

> [https://huggingface.co/evolve-build/face_recognition](https://huggingface.co/evolve-build/face_recognition)

## 2. Place Weights in the Correct Folders

After downloading, organize the weights into the following directories:

- **ArcFace model weights** ➔  
  `facerecognition/arcface/weights/`
  
- **SCRFD face detection weights** ➔  
  `face_detection/scrfd/weights/`
  
- **YOLOv5 Face detection weights** ➔  
  `face_detection/yolov5_face/weights/`

> ⚡ Ensure the folders are correctly named and placed for smooth execution!

## 3. Capture Reference Images

Run the following command to capture 5 reference images by pressing c to click photo of the face you want to recognize:

```bash
python capture_refs.py
```

These photos get stored in datasets/target_person

## 4. Run Detection

After capturing the reference images, start the detection process by running:

```bash
python detect.py
```
