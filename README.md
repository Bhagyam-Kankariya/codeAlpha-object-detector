codeAlpha-object-detector

A simple Flask-based web application for real-time object detection using a pre-trained YOLOv8 model. This project lets users upload images via a web interface and returns detections with bounding boxes and labels drawn on the image.

🚀 Features

🔍 Object Detection using YOLOv8 (ultralytics model).

🖼️ Web Interface built with Flask.

📤 Upload images and get predictions in real time.

📦 Includes model weights (yolov8n.pt) for inference.

📁 Repository Structure
codeAlpha-object-detector/
├── templates/             # HTML templates for the web app
├── app.py                 # Main Flask application
├── yolov8n.pt             # Pretrained YOLOv8-nano model weights
└── README.md              # Project overview and instructions

🛠️ Prerequisites

Make sure you have the following installed on your system:

Python 3.8+

pip

Also install the necessary Python packages:

pip install -r requirements.txt


If you don’t have a requirements.txt, create one with:

flask
ultralytics
opencv-python
numpy

📌 How It Works

The Flask app (app.py) serves a web page for uploading images.

When an image is submitted:

It’s passed to the YOLOv8 model (yolov8n.pt) for inference.

Objects are detected and bounding boxes drawn.

The result is displayed back to the user.

🔍 Usage
1. Clone the repository
git clone https://github.com/Bhagyam-Kankariya/codeAlpha-object-detector.git
cd codeAlpha-object-detector

2. Run the Flask app
python app.py


You should see something like:

 * Running on http://127.0.0.1:5000/

3. Open in Browser

Visit:

http://127.0.0.1:5000/


Upload an image and the app will show detected objects.

📦 Model Info

This project uses the YOLOv8n (nano) model—a lightweight, real-time object detector suitable for CPU inference. The weights file yolov8n.pt is included so you can run the detector without additional downloads.

📌 Notes & Tips

For better performance or more classes, swap in a larger YOLOv8 model (e.g., yolov8s.pt, yolov8m.pt).

If running on GPU, make sure PyTorch with CUDA support is installed for faster inference.

🎯 Contributing

Contributions are welcome! You can:

Add support for video uploads or webcam detection

Add downloadable output images

Improve UI/UX

Just fork, branch, commit, and open a PR.

