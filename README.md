# facial-shape-detection

This project uses Dlib and OpenCV to detect facial landmarks and classify face shapes. The script analyzes an input image to determine whether the face shape is Oval, Round, Square, or Unknown based on specific geometric ratios.

# Features
1. Facial Landmark Detection:
Identifies 68 key facial landmarks using Dlib's pre-trained model (shape_predictor_68_face_landmarks.dat).
2. Face Shape Classification:
Classifies face shapes based on:
Cheekbone width to face length ratio.
Jawline length to face length ratio.
3. Visualization:
Displays the image with facial landmarks (if using Colab or similar environments).

# Installation
1. Clone the Repository
git clone [https://github.com/your-repo-name/face-shape-detection.git](https://github.com/nehaatri1997/facial-shape-detection/blob/main/face_shape_detection.py)
cd face-shape-detection
2. Install Required Libraries
Install the necessary dependencies:
pip install opencv-python dlib numpy requests

# Usage
1. Download the Pre-Trained Model
The script downloads the required model (shape_predictor_68_face_landmarks.dat) automatically. Ensure you have an internet connection.
2. Run the Script
Replace the image_path in the script with the path to your image file. Then, execute:
python face_shape_detection.py
3. Output
The script prints the detected face shape for each face in the image.

Example output:
Detected facial shape: Oval

# File Structure
face_shape_detection/
│
├── face_shape_detection.py    # Main Python script for face shape detection
├── README.md                  # Documentation file
└── requirements.txt           # List of dependencies (optional)

# Customization
1. Change Image Input:
Replace the image_path variable with your desired image file path.
image_path = "path/to/your/image.jpg"
2. Add Visualization:
Use cv2.imshow or cv2.imwrite to save or display results locally.

# Limitations
1. Requires clear, frontal face images for accurate detection.
2. Performance depends on the quality and angle of the input image.
3. Classification is limited to Oval, Round, Square, or Unknown.

# Future Enhancements
1. Real-time face shape detection using a webcam.
2. Integration with facial expression detection for combined analysis.
3. Improve classification accuracy by refining the geometric rules.
