#  Smart Trash Detector (YOLOv8 + Custom Classifier)

A real-time AI system to detect and classify trash items using **YOLOv8** for object detection and a custom-trained **MobileNetV2 classifier** for waste category prediction.

 The app uses your webcam to detect trash items live and overlays the predicted category (e.g., plastic, glass, paper) with confidence scores.

---

##  Features

 Real-time detection of trash using YOLOv8.  
 Classification of detected regions into 6 categories:  
- **cardboard**
- **glass**
- **metal**
- **paper**
- **plastic**
- **trash**

 Bounding boxes with predicted class labels and confidence.  
 Runs smoothly on CPU, faster with GPU.  
 Modular code – easy to extend or retrain.

---


##  Folder Structure

Smart-Trash-Detector/
├── classifier/
│ ├── waste_classifier.h5 # Trained MobileNetV2 model
│ ├── train_classifier.ipynb # Jupyter notebook for training
├── detector/
│ ├── live_trash_detector.py # Live camera YOLO + classifier script
│ ├── yolov8n.pt # YOLOv8 pre-trained weights
├── demo/
│ ├── live_detection.gif # Demo video/gif
│ ├── prediction.jpg # Sample prediction image
├── README.md
├── requirements.txt

yaml
Copy
Edit

---

##  Installation

###  Clone the repository
```bash
git clone https://github.com/your-username/Smart-Trash-Detector.git
cd Smart-Trash-Detector
 Install dependencies
bash
Copy
Edit
pip install -r requirements.txt
requirements.txt

nginx
Copy
Edit
tensorflow
opencv-python
ultralytics
numpy
matplotlib
 Download YOLOv8 weights
YOLOv8 Nano weights are automatically downloaded when running the script. Or download manually from Ultralytics.
