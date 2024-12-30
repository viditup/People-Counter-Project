# People Counter Project

Welcome to the **People Counter Project**. This project aims to detect and count people in real-time using **YOLO** (You Only Look Once) object detection. It processes video streams and recorded footage, providing a live count of people within the frame. This system is optimized for GPU acceleration with **CUDA** support to ensure fast and accurate real-time performance.

---

### **Overview**

The **People Counter** system is designed to detect and track people in video streams using the **YOLO** object detection model. It is ideal for applications such as crowd monitoring, security, or public space analysis. The system uses **PyTorch** and **OpenCV** for video processing and real-time object detection. Additionally, it leverages **CUDA** for improved performance on machines with compatible NVIDIA GPUs.

---

### **Features**

- **Real-Time People Counting**: Detect and count people in video streams with minimal latency.
- **CUDA Acceleration**: Uses **CUDA** for optimized GPU performance, allowing for faster inference.
- **Accurate Tracking**: Utilizes YOLO for detecting and tracking people in video frames.
- **Customizable**: Adapt the script to work with various video sources (e.g., webcam, recorded video).
- **Easy Integration**: Plug-and-play setup for quick implementation in any Python environment.

---

### **Tech Stack and Requirements**

This project requires several libraries and tools to run effectively:

#### **Required Libraries**:
Ensure the following libraries are installed:
```bash
pip install -r requirements.txt
```

- **cvzone**: 1.5.6
- **ultralytics**: 8.0.26 (YOLO implementation)
- **hydra-core**: >=1.2.0
- **matplotlib**: >=3.2.2
- **numpy**: >=1.18.5
- **opencv-python**: 4.5.4.60
- **Pillow**: >=7.1.2
- **PyYAML**: >=5.3.1
- **requests**: >=2.23.0
- **scipy**: >=1.4.1
- **torch**: >=1.7.0
- **torchvision**: >=0.8.1
- **tqdm**: >=4.64.0
- **filterpy**: 1.4.5
- **scikit-image**: 0.19.3
- **lap**: 0.4.0

#### **System Requirements**:
- **CUDA**: Ensure you have a compatible NVIDIA GPU with CUDA installed for hardware acceleration.
- **PyTorch with CUDA**: Install the correct version of PyTorch for GPU support:
  ```bash
  pip install torch torchvision torchaudio
  ```

---

### **Project Structure**

```bash
People-Counter/
├── __pycache__/
├── graphics.png
├── mask.png
├── people-Counter.py
├── sort.py
├── README.md
└── requirements.txt
```

---

### **How to Run the Code**

Follow these steps to run the **People Counter** script:

1. **Install Dependencies**:
   Ensure all required libraries are installed by running:
   ```bash
   pip install -r requirements.txt
   ```

2. **Run the People Counter Script**:
   Execute the script using the following command:
   ```bash
   python people-Counter.py
   ```

3. **Input Source**:
   - For **real-time webcam detection**, ensure your webcam is connected.
   - For **video file input**, place your video in the same directory as the script or update the file path in the code.

4. **YOLO Model Weights**:
   Ensure the **YOLO model weights** are available and properly configured for the script.

---

### **Project Demonstrations**

Below are some images showcasing how the **People Counter** system works in real-time.

#### **Example of People Counting in Real-Time**

This example shows how the system detects and counts people in a live video stream.

![Screenshot 2024-12-30 180834](https://github.com/user-attachments/assets/8f239874-b49c-48b5-972d-d821936f365a)
![Screenshot 2024-12-30 180947](https://github.com/user-attachments/assets/cec07d10-283b-4273-a930-865978136b85)
![Screenshot 2024-12-30 181036](https://github.com/user-attachments/assets/e8ab3c8e-e6a4-47a4-90e6-a8a3078b15ea)
![Screenshot 2024-12-30 181202](https://github.com/user-attachments/assets/0f9a1a1a-f2b9-4940-acf8-c6289d31e877)

#### **Real-Time Graphics Display**

The system displays bounding boxes and tracking information to help visualize the detected people.

![graphics](https://github.com/user-attachments/assets/ef112aae-303a-492e-8c91-98ef27d93d4c)

#### **Mask Image for Preprocessing**

This mask image helps with preprocessing and detecting where people are most likely to appear in the video frame.

![mask](https://github.com/user-attachments/assets/5d2d05f2-9bd5-4515-89c7-07ee9a6d0e0f)

---

### **People Counter Components**

#### **Key Files**:
- **`people-Counter.py`**: The main Python script for people detection and counting. It processes the video feed, applies YOLO for object detection, and tracks the number of people in each frame.
- **`sort.py`**: Implements the sorting algorithm to track people across frames and ensure the correct count of unique individuals.
- **`graphics.png`**: A reference image used to visualize the counting process, overlaying graphics on the video stream.
- **`mask.png`**: A preprocessing mask to highlight areas where people are likely to appear in the frame.

---

### **Contributing**

We welcome contributions to improve and expand this project. To contribute:

1. Fork the repository.
2. Create a new feature branch (`git checkout -b feature-name`).
3. Implement your changes and thoroughly test them.
4. Push your changes to your fork (`git push origin feature-name`).
5. Open a pull request with a description of the changes.

---

### **License**

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for more details.

---

### **Acknowledgments**

- **YOLO**: For providing an efficient and fast object detection model.
- **OpenCV**: Used for real-time video processing and frame handling.
- **PyTorch**: Used for model inference and GPU acceleration.

---

### **Contact**

If you have any questions or need support, feel free to open an issue on the GitHub repository or contact me directly at viditupadhyay07@gmail.com.

---
