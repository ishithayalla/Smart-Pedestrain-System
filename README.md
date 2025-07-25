**Smart Pedestrian and Vehicle Detection System 🚦🚶‍♂️🚗**


This project uses MobileNet-SSD, a pre-trained deep learning model, to detect persons and vehicles in a video and simulate a smart signaling system (like traffic lights) based on majority detection.

📌 Overview
The system:

Takes a video input.

Detects objects frame-by-frame using MobileNet-SSD.

Counts the number of persons and vehicles in each frame.

Displays a green, red, or yellow circle to simulate a traffic signal based on which group is in majority.

Generates an output video with bounding boxes, labels, and signal indicators.

🧠 Features
Real-time object detection using OpenCV DNN module.

Pre-trained model (MobileNetSSD) for fast and lightweight inference.

Simple decision-making logic to simulate smart signal control.

Colored indicator and message overlay for better visualization.

🛠️ Technologies Used
Python

OpenCV

MobileNet-SSD (Caffe model)

Google Colab (for demo and execution)

📽️ How It Works
Upload a video file via Colab.

The script processes every alternate frame:

Detects objects like person, car, bus, motorbike, etc.

Counts detected persons and vehicles.

Adds bounding boxes and confidence scores.

Displays signal indicator (green/red/yellow) based on counts.

Saves and downloads the processed output video.

📁 Files
MobileNetSSD_deploy.prototxt – Model configuration file.

MobileNetSSD_deploy.caffemodel – Pre-trained weights.

output_video_with_signal.mp4 – Resulting video with detections and signal logic.

🖼️ Example Output
🟢 More persons → All clear!
🔴 More vehicles → Stay safe!
🟡 Equal → Proceed with caution!

🚀 Run It on Google Colab
Upload your video.

Run the notebook cells (model download, processing, and download output).

View or share the generated video.

📈 Possible Extensions
Switch to YOLOv8 or SSD with TensorFlow Lite for improved performance.

Add a dashboard or logging system to track detection statistics.

Implement real-time webcam-based detection.
