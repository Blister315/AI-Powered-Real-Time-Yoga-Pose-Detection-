**Yoga Pose Detection Using AI**

This project is an AI-powered yoga assistant that detects and classifies yoga poses in real time using a webcam. The system uses MoveNet for pose estimation and a trained machine learning model to identify various yoga postures.

**Overview**

The application helps users practice yoga correctly without needing a physical instructor. By analyzing the user’s body posture and detecting joint positions, the model predicts which yoga pose is being performed.

** How It Works**

User stands in front of the camera.

MoveNet detects 17 body keypoints (like shoulders, hips, knees, etc.).

The trained classifier analyzes these points.

The system recognizes which yoga pose is being performed.

**Project Structure**
AI Yoga Coach Project
│
├── yoga_poses/           # Dataset (train/test)
├── data.py              # Pose representation and keypoint structure
├── preprocessing.py     # Extracts MoveNet keypoints and generates CSV
├── training.py          # Trains ML model and exports to TensorFlow.js
├── src/                 # React front-end app
└── public/              # Web UI assets

**Supported Yoga Poses**

Mountain Pose

Tree Pose

Cobra Pose

Triangle Pose

Warrior Pose

Child Pose

Downward Dog

One-Legged Chair Pose

**Technologies Used**
Component	Usage
TensorFlow & TensorFlow.js	Model training and browser prediction
MoveNet (Google AI)	Pose estimation and keypoint detection
Python	Data preprocessing and model training
React.js	Front-end user interface
Scikit-Learn	Data splitting and utilities

**Setup Instructions
**1️⃣ Install Python Dependencies
pip install -r requirements.txt

2️⃣ Run Preprocessing
python preprocessing.py

3️⃣ Train the Model
python training.py

4️⃣ Start Web Application
npm install
npm start

**Model Training Details**

Type: Dense Neural Network

Loss: Categorical Crossentropy

Optimizer: Adam

Epochs: 200

Output Activation: Softmax

**Future Improvements**

Voice-based feedback for pose correction

Real-time accuracy percentage

Support for multiple users at once

Mobile application version

Additional yoga pose categories

.
