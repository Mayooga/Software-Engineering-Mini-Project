# Traffic Detector v2

A Python-based traffic violation detection application using YOLOv8 for real-time analysis of video streams. It identifies risky behaviors such as speeding, erratic maneuvers, and phone use while driving, providing violation reports.

## Features

- Real-time traffic violation detection (speeding, risky maneuvers, distracted driving)
- Supports video files 
- Uses YOLOv8 nano model for efficient object detection
- Web interface built with Flask for uploading and viewing results
- Generates JSON reports of detected violations with recommendations

## Installation

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Download the YOLOv8 model:
   - Download `yolov8n.pt` from the [Ultralytics YOLOv8 releases](https://github.com/ultralytics/ultralytics/releases) or use the official download script.
   - Place the model file in the project root directory.

## Usage

1. Run the application:
   ```bash
   python app.py
   ```

2. Open your browser and navigate to `http://localhost:5000`

3. Upload a video or image file for detection.

## Project Structure

- `app.py`: Main Flask application
- `detect.py`: Detection logic using YOLOv8
- `requirements.txt`: Python dependencies
- `yolov8n.pt`: YOLOv8 model (download separately)
