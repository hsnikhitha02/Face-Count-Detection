# Face Count Detection

## Overview

Face Count Detection is a computer vision-based monitoring module developed using Python and OpenCV. The system captures live video from a webcam, detects human faces in each frame, counts the number of faces present, and displays the count in real time.

This module can be integrated into online monitoring systems to identify situations where multiple individuals are present in front of the camera.

---

## Objective

The objective of this project is to:

- Detect all visible human faces in a webcam frame.
- Count the number of detected faces.
- Display the face count in real time.
- Provide structured output for integration with monitoring systems.

---

## Features

- Real-time webcam face detection
- Face counting functionality
- Bounding box visualization
- Live face count display
- Lightweight and fast execution
- Easy integration with monitoring modules

---

## Technologies Used

- Python
- OpenCV
- Haar Cascade Classifier
- Visual Studio Code

---

## Project Structure

```text
Face_Count_Detection/
│
├── face_count.py
├── README.md
├── test_images/
│   ├── one_face.jpg
│   ├── two_faces.jpg
│   └── three_faces.jpg
│
├── output/
│   └── screenshots
│
└── report/
    └── Face_Count_Detection_Report.docx
```

---

## Installation

### Clone the Repository

```bash
git clone <repository-link>
cd Face_Count_Detection
```

### Install Dependencies

```bash
pip install opencv-python
```

---

## Running the Project

Execute the following command:

```bash
python face_count.py
```

The webcam window will open automatically.

Press **ESC** to exit the application.

---

## Working Process

1. Initialize webcam.
2. Capture video frames.
3. Convert frames to grayscale.
4. Detect faces using Haar Cascade.
5. Count detected faces.
6. Display face count.
7. Show bounding boxes around detected faces.

---

## Sample Output

### One Face

```json
{
  "face_count": 1
}
```

### Two Faces

```json
{
  "face_count": 2
}
```

### Three Faces

```json
{
  "face_count": 3
}
```

---

## Testing

The system was tested under the following scenarios:

| Test Case | Expected Result |
|------------|----------------|
| No Face | 0 Faces |
| One Face | 1 Face |
| Two Faces | 2 Faces |
| Three Faces | 3 Faces |
| Multiple Faces | Accurate Count |

---

## Challenges

### MediaPipe Compatibility Issue

MediaPipe generated compatibility issues with Python 3.13.

### Solution

The implementation was switched to OpenCV Haar Cascade Face Detection, which provided stable and reliable performance.

---

## Results

- Successfully detected faces in real time.
- Correctly counted visible faces.
- Achieved more than 90% accuracy under normal lighting conditions.
- Met all project requirements.

---

## Future Enhancements

- Face recognition support
- Anti-spoofing detection
- Reflection filtering
- Poster and screen face filtering
- Deep learning-based face detection
- Integration with monitoring dashboards

---

## License

This project is developed for educational and internship purposes.
