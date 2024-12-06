# Licence-Plate-Detection-and-Recognition-using-YOLO-V8-EasyOCR

---

# License Plate Detection and Recognition  

This repository contains the implementation of a License Plate Detection and Recognition system. The project uses YOLOv8 for license plate detection and EasyOCR for character recognition, for real-time processing of videos or images to detect and recognize license plate numbers.  

## Overview  
This project focuses on accurately detecting and recognizing license plates under varying environmental conditions.  
- **Detection:** Uses YOLOv8, a state-of-the-art object detection model, fine-tuned on an annotated license plate dataset.  
- **Recognition:** Leverages EasyOCR for extracting alphanumeric characters from the detected license plates.  

## Features  
- Real-time license plate detection and recognition.  
- Supports video input (broken into frames) and image input.  
- Preprocessing steps to enhance image quality.  
- Fine-tuning and augmentation for improved accuracy.  
- Evaluation against labeled datasets to calculate performance metrics.  

## Architecture  
The project pipeline consists of the following steps:  
1. **Frame Extraction:** Videos are split into frames using OpenCV.  
2. **Detection:** YOLOv8 detects license plates in frames.  
3. **Preprocessing:** Enhances plate images for recognition (e.g., noise removal, resizing).  
4. **Recognition:** EasyOCR extracts alphanumeric characters from the detected plates.  
5. **Validation:** Results are compared with ground truth to compute accuracy.


## Dataset  
The model was fine-tuned on a custom dataset of license plates, annotated using [LabelImg](https://github.com/heartexlabs/labelImg).

## Results 
- **Accuracy:** Achieved an accuracy of near 99% for character recognition, given the small dataset, could a,so be very accurate for a larger dataset.  
- The system successfully detects and recognizes plates under varying conditions, including low light and different plate designs.  

## Future Improvements  
- Expand the dataset with more diverse license plate styles and regions.  
- Optimize the model for edge devices.  
- Add multilingual recognition support(EasyOCR already supports this) 
- Implement hyperparameter tuning to improve edge-case performance.  

## Acknowledgments  
- [Ultralytics YOLOv8](https://github.com/ultralytics/yolov8) for the object detection framework.  
- [EasyOCR](https://github.com/JaidedAI/EasyOCR) for text recognition.  
- Inspiration from Rayudu Sushma's work in OCR and detection systems.  

--- 
