# Sustainable Traffic Monitoring and Management

This project is a Python-based system for vehicle detection and counting using video footage. It employs computer vision techniques with OpenCV to monitor traffic flow, count vehicles, and support sustainable traffic management.

## 📁 Project Structure

| File        | Description |
|-------------|-------------|
| `vehicle.py` | Main Python script to detect and count vehicles using a video input. |
| `video.mp4` | Sample input video for vehicle detection and analysis. |

## 🧠 Features

- Vehicle detection using background subtraction
- Vehicle counting using virtual lines
- Frame resizing for standard resolution
- Works with pre-recorded video (`.mp4`)

## ⚙️ Requirements

- Python 3.x
- OpenCV (including `opencv-contrib-python` for `bgsegm`)

Install dependencies:

```bash
pip install opencv-python opencv-contrib-python
```

## 🚀 How to Run

1. Make sure `vehicle.py` and `video.mp4` are in the same directory.
2. Run the script:

```bash
python vehicle.py
```

3. The video window will display:
   - Bounding boxes around detected vehicles
   - A line for vehicle counting
   - Real-time vehicle counter displayed on the video

Press `Enter` key to stop the video and close all windows.

## 📈 Methodology

- Convert frames to grayscale and apply Gaussian blur
- Apply background subtraction using MOG (Mixture of Gaussians)
- Morphological operations to clean up the mask
- Draw a virtual line to count vehicles that cross it
- Update and display a real-time counter

## 📄 License

This project is for educational and research purposes.
#
