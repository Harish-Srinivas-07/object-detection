# Object Detection using YOLO version 3

🚀 Welcome to the Object Detection using YOLOv3 tutorial! In this guide, we'll walk you through the process of setting up and using YOLOv3 to detect objects in images and perform real-time object detection in videos.

## 📦 Import Details

Make sure you have the following dependencies installed:

- OpenCV
- NumPy
- Matplotlib
- Jupyter Lab

You can install them using the following command:

```bash
pip install opencv-python numpy matplotlib jupyterlab
```

## 📚 Introduction

You Only Look Once (YOLO) is a state-of-the-art, real-time object detection algorithm. YOLOv3, the latest version, will be applied to detect objects in images. A set of pre-trained weights, based on the Common Objects in Context (COCO) database, is utilized for this tutorial.

## 🖼️ Actual Data

We encourage you to test the YOLO algorithm on your images. The provided images are:

- cat.jpg
- city_scene.jpg
- dog.jpg
- dog2.jpg
- eagle.jpg
- food.jpg
- giraffe.jpg
- horses.jpg
- motorbike.jpg
- person.jpg
- surf.jpg
- wine.jpg

These images are located in the `./images/` folder.

## 🛠️ Installation

Follow these steps to set up the YOLOv3 environment:

1. Clone the repository:

   ```bash
   git clone https://github.com/Harish-Srinivas-07/object-detection.git
   ```

2. Navigate to the project directory:

   ```bash
   cd yolov3-object-detection
   ```

3. Download the YOLOv3 weights, configuration, and COCO object classes file:

   - [yolov3.cfg](https://github.com/Harish-Srinivas-07/object-detection/blob/main/cfg/yolov3.cfg)
   - [yolov3.weights](https://pjreddie.com/media/files/yolov3.weights)
   - [coco.names](https://github.com/Harish-Srinivas-07/object-detection/blob/main/data/coco.names)

4. Run the YOLOv3 object detection:

   ```bash
   jupyter lab detection.ipynb
   ```

## 🤖 Theory

### YOLOv3 Architecture

The neural network used by YOLOv3 consists mainly of convolutional layers, with shortcut connections and upsample layers.

### Non-Maximal Suppression

YOLO uses Non-Maximal Suppression (NMS) to keep the best bounding box. Set the NMS threshold to 0.6 to remove predicted boxes with low probability.

### Intersection Over Union

IOU is used to select the best bounding boxes. Set the IOU threshold to 0.4 to eliminate overlapping boxes.

## 🎥 Video Analysis

To perform object detection in videos:

1. Load the pre-trained model and classes.
2. Initialize video capture (from camera or file).
3. Apply YOLOv3 to each frame, filter detections, and apply NMS.
4. Display results in the 'Tracking' window.
5. Press 'q' to exit the program.

Adjust parameters such as `weight_file`, `cfg_file`, `namesfile`, `iou_thresh`, and `nms_thresh` as needed.

```bash
jupyter lab detection.ipynb -> final phase
```

## 📊 Jupyter Lab Integration

To use YOLOv3 in Jupyter Lab:

1. Launch Jupyter Lab:

   ```bash
   jupyter lab
   ```

2. Open the provided `detection.ipynb` notebook.

3. Run the cells in the notebook to perform object detection interactively.

Have fun exploring the world of YOLOv3 object detection! 🕵️‍♂️
