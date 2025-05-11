---

# Urban Traffic Tiny Object Detection via Attention and Multi-Scale Feature Driven in UAV-Vision

## Overview

This project focuses on enhancing tiny object detection in urban traffic using Unmanned Aerial Vehicles (UAVs). UAVs are increasingly utilized for remote monitoring in sensitive or urban areas to ensure public safety. However, UAVs often struggle to detect and recognize small objects, which can lead to detection failures. This project introduces a novel algorithm called **RTS-NET (Real-time Small Object Detection Network in UAV-Vision)**, designed to improve the accuracy and speed of small object detection in UAV-vision systems.

## Key Features

* **RTS-NET** combines three CNN layers:

  * **MFFM** (Multi-Scale Feature Fusion Module) to enhance feature scaling.
  * **Attention CADM** (Class-Aware Discriminative Module) to differentiate between background and real objects.
  * **RFEM** (Real-time Feature Extraction Module) to speed up detection and reduce prediction time.
* The algorithm outperforms existing models like **YOLOv5** to **YOLOv8** and **Efficient-Net** in terms of detection accuracy.

## Dataset

The algorithm is trained on a custom traffic vehicle dataset captured from UAV drones. The dataset consists of 8 vehicle classes such as cars, bikes, trucks, and pedestrians. Due to its uniqueness, the dataset is not publicly available, but a similar dataset with 4 car models (0 to 3) is available for download [here](https://universe.roboflow.com/object-detection-vwva6/vehicle-detection-in-aerial-images).

## Usage

1. Prepare the dataset by downloading the UAV vehicle detection dataset.
2. Train the model with the dataset.
3. Test the model on test data to evaluate performance.

## Results

The **RTS-NET** model significantly improves small object detection accuracy when compared to traditional models. The project demonstrates its effectiveness in real-world urban traffic scenarios using UAVs.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

