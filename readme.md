 Parking Space Detection using OpenCV

A simple Parking Management System using Python and OpenCV that detects whether parking spaces are **occupied or empty** using image processing (no ML used).

---

## 📌 Features

- Detects free & occupied parking spots in a video
- Manual slot selection using mouse clicks
- Real-time detection with color-coded boxes (green = free, red = occupied)
- Saves output video with overlays

---

## 🧠 How It Works

1. **Manual Setup (`get_first_frame& save_polygon_positions.py`)**:
   - Loads a sample image from video.
   - Click to mark top-left corners of slots.
   - Press `s` to save positions.

2. **Detection (`Main_results_check.py`)**:
   - Loads saved slot positions.
   - Processes each frame using grayscale, blur, threshold.
   - Detects white pixel count to determine occupancy.
   - Draws rectangles and shows count of free slots.