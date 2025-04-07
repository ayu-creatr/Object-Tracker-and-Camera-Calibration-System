# 🎯 Object Tracker & Camera Calibration using OpenCV

A computer vision project built with Python and OpenCV to **calibrate cameras** using Zhang's method and **track objects** in real-time based on user-defined quadrilateral regions. The system includes GUI-based point selection, pose estimation with rotation matrix to Euler angle conversion, and visual tracking using perspective transforms.

---

## 🚀 Features

- 📷 **Camera Calibration**  
  Calibrate intrinsic and extrinsic camera parameters using a checkerboard pattern with Zhang's method.

- 🎯 **Object Tracking**  
  Track quadrilateral regions in real-time with accurate perspective transformation.

- 🎮 **Interactive ROI Selection**  
  Select the region of interest by clicking 4 points on the video/image interface.

- 🔁 **3D Pose Estimation**  
  Convert rotation matrices to Euler angles (yaw, pitch, roll) with gimbal lock handling.

- 🧰 **Built with Python + OpenCV**  
  Modular, well-commented code with clean logic separation.

---

## 🧩 Modules

| File | Description |
|------|-------------|
| `zhang.py` | Calibrates camera using checkerboard images (Zhang’s method) |
| `function.py` | Utility functions for drawing and angle conversions |
| `tracker.py` | Main script to run object tracking with ROI selection |

---

### 🎯 Camera Calibration Output

Camera Matrix: [ fx 0 cx ] [ 0 fy cy ] [ 0 0 1 ]



---

## ⚙️ How to Run

1. **Clone the repository**

```bash
git clone https://github.com/your-username/object_tracker.git
cd object_tracker
```

2. Install dependencies
   ```bash
   pip install -r requirements.txt
   pip install opencv-python numpy
   ```
3. Run camera calibration
Make sure your checkerboard images are in ./images/

```bash
  python zhang.py
```

4. Run object tracker
   ```bash
   python tracker.py
   ```

🖼 Sample Output
➕ Selected ROI
User selects 4 points:


✅ Tracked Object

💡 Future Improvements
-Add multi-object tracking support

-Save/load calibration parameters

-Real-time video stream tracking

-Export tracking data (e.g., coordinates, angle)

🧑‍💻 Author
Ayush Goyal
LinkedIn[https://www.linkedin.com/in/ayush-goyal-617893281]


