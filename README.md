# Face Recognition Based Attendance System

A Python GUI application for marking attendance using face recognition technology. The system captures face images, trains a face recognizer, and tracks attendance by recognizing faces in real-time using a webcam.

---

## Features

- Capture multiple images of a person to build the training dataset.
- Train a face recognizer (LBPH algorithm) on collected images.
- Real-time face detection and recognition to mark attendance.
- Attendance records saved as timestamped CSV files.
- Simple Tkinter GUI interface for user interaction.

---

## Technologies & Libraries Used

- Python 3.x
- OpenCV (`cv2`)
- Tkinter for GUI
- NumPy
- Pandas
- Pillow (PIL)
- CSV module
- Haar Cascades for face detection

---

## File Structure

- `haarcascade_frontalface_default.xml` - Haar cascade classifier for face detection.
- `TrainingImages/` - Folder to store captured face images.
- `TrainingImageLabel/Trainer.yml` - Trained model saved after training.
- `StudentDetails/StudentDetails.csv` - CSV file to store ID and Name.
- `ImagesUnknown/` - Folder to store unknown face images detected during recognition.
- `Attendance/` - Folder to save attendance CSV files.

---

## How to Use

1. **Enter ID and Name** in the GUI and click **UPLOAD IMAGE** to capture images.
2. Click **TRAINER** to train the model on the captured images.
3. Click **MARK YOUR ATTENDANCE** to start real-time face recognition and mark attendance.
4. Attendance will be saved automatically as a CSV file in the `Attendance/` folder.
5. Use **Clear** buttons to clear the ID or Name fields.
6. Click **Quit** to exit the application.

---

## Requirements

Install the required Python libraries:

```bash
pip install opencv-python numpy pandas pillow

