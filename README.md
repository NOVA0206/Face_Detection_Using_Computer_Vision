## Face Detection Using Computer Vision

This repository contains two Python scripts that perform face detection using [OpenCV](https://opencv.org/) and Haar Cascade Classifiers.  
It supports both **static image detection** and **real-time camera-based detection**.

## 📂 Repository Contents

- **`face_detection_from_photo.py`** — Detects faces in a static image (`Jeevan.jpg` included in the repo).
- **`face_detection_live.py`** — Detects faces in real-time using your webcam and outputs the number of faces detected in the terminal.
- **`haarcascade_frontalface_default.xml`** — Pre-trained Haar Cascade model used for detecting faces.
- **`Jeevan.jpg`** — Sample image for testing static face detection.

---

## 🚀 Features

- **Static Image Detection**  
  Detects faces from a given photo and marks them with bounding boxes.

- **Live Face Detection**  
  Captures video from the webcam in real-time and:
  - Detects faces frame-by-frame
  - Prints the number of faces detected in the terminal
  - Displays live camera feed with bounding boxes around detected faces

- **Haar Cascade Model**  
  Uses OpenCV’s `haarcascade_frontalface_default.xml` for accurate frontal face detection.

---

## 📦 Installation

Make sure you have **Python 3.7+** installed.

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/Face_Detection_Using_Computer_Vision.git
   cd Face_Detection_Using_Computer_Vision


2. Install dependencies:

   ```bash
   pip install opencv-python
   ```

---

## 🖼 Static Face Detection

Run:

```bash
python face_detection_from_photo.py
```

* The script will load `Jeevan.jpg` (or your own image if you change the filename in the script).
* A window will appear with detected faces marked by rectangles.

---

## 🎥 Live Face Detection

Run:

```bash
python face_detection_live.py
```

* Uses your default webcam (index `0`) to capture live video.
* Prints number of detected faces in the terminal.
* Displays video feed with bounding boxes.

> **Note:** If you get a "camera index out of range" error, try changing:
>
> ```python
> cv2.VideoCapture(0)
> ```
>
> to:
>
> ```python
> cv2.VideoCapture(1)  # or higher index
> ```

---

## 📄 Haar Cascade Classifier

We use OpenCV’s built-in Haar Cascade XML:

```
haarcascade_frontalface_default.xml
```

This model detects frontal human faces efficiently.

---

## ⚖ License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙌 Acknowledgements

* [OpenCV](https://opencv.org/) — Computer vision library
* Haar Cascade Classifiers — Original work by Viola and Jones

✉️ Contact For any questions or inquiries, reach out to:

Author: Jeevan Ramesh Jadhav Email: jeevanj020604@gmail.com
LinkedIn: https://www.linkedin.com/in/jeevanjadhav02/
Github Username: NOVA0206

Built with ❤️ using Power BI.
