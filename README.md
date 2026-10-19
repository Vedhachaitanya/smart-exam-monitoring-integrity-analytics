# Smart Exam Monitoring & Integrity Analytics Platform

A computer vision-based project that monitors exam sessions using a webcam, detects faces, records monitoring events, and displays event summaries through a Streamlit dashboard.

## About the Project

The Smart Exam Monitoring & Integrity Analytics Platform is developed using Python and OpenCV. It captures webcam frames and detects faces to identify basic monitoring states such as one face detected, no face detected, and multiple faces detected.

The system records monitoring events in a CSV file and displays event summaries through a Streamlit dashboard.

**Note:** Monitoring events are indicators for review, not proof of cheating.

## Objectives

- Detect faces using a webcam.
- Identify no-face, one-face, and multiple-face states.
- Record monitoring events with timestamps.
- Display monitoring summaries using a dashboard.
- Learn computer vision, image processing, and data analytics.

## Technologies Used

- **Python** — main programming language
- **OpenCV** — webcam and image processing
- **Haar Cascade Classifier** — face detection
- **NumPy** — numerical operations
- **Streamlit** — interactive dashboard
- **Pandas** — event data processing
- **CSV** — monitoring event storage

## Features

- Webcam-based face detection
- Face count monitoring
- Detection-state event logging
- Timestamped CSV event history
- Streamlit dashboard for monitoring summaries
- Event counts for one face, no face, and multiple faces

## Project Workflow

1. Capture video frames from the webcam.
2. Process the frames using OpenCV.
3. Convert frames to grayscale for face detection.
4. Detect faces using the Haar Cascade classifier.
5. Count the detected faces.
6. Identify the current monitoring state.
7. Record relevant state changes in a CSV file.
8. Display event summaries in the Streamlit dashboard.

## Project Structure

```text
SmartExamMonitoring/
├── face_detection.py
├── exam_monitor.py
├── dashboard.py
├── requirements.txt
├── README.md
├── .gitignore
└── screenshots/
```

*Note: This is the expected structure. Keep the actual filenames and folders used in your repository.*

## Requirements

- Python 3.13 (or another compatible version)
- Webcam
- Visual Studio Code (recommended)
- Required Python packages

## Installation and Setup

### 1. Clone the Repository

```bash
git clone YOUR_REPOSITORY_URL
cd YOUR_REPOSITORY_FOLDER
```

Replace the example values with your actual GitHub repository URL and folder name.

### 2. Create a Virtual Environment

For Windows:

```powershell
py -3.13 -m venv .venv
.\.venv\Scripts\Activate.ps1
```

### 3. Install Dependencies

```powershell
python -m pip install -r requirements.txt
```

## How to Run the Project

### Run Face Detection

```powershell
python face_detection.py
```

### Run Exam Monitoring

```powershell
python exam_monitor.py
```

### Run the Streamlit Dashboard

```powershell
python -m streamlit run dashboard.py
```

Use a webcam for the face detection and exam monitoring programs. The dashboard reads the monitoring data according to the configuration in the project code.

## Expected Output

- Webcam window showing face detection
- Face count and monitoring states
- CSV file containing recorded monitoring events
- Dashboard showing event totals and event history

## Limitations

- Face detection does not verify a person's identity.
- A monitoring event does not prove cheating or misconduct.
- Lighting, camera quality, and face position may affect detection accuracy.
- This project is a learning prototype and is not a replacement for human review.

## Future Enhancements

- Live alerts for no-face detection
- Live alerts for multiple-face detection
- Exam session start and end management
- Improved event analytics and visualizations
- Better testing under different lighting conditions

## Privacy and Responsible Use

Use this project with appropriate consent when capturing webcam data. Avoid publishing personal recordings, sensitive student information, or private monitoring logs in the public repository.

## Project Status

The current implementation includes webcam face detection, CSV event logging, and a Streamlit dashboard. Additional monitoring and alert features can be developed in future versions.

## Author and Team

Developed as a BTech IT project to explore Python, computer vision, OpenCV, and analytics.

Add the group members' names here if approved by the team.

## Disclaimer

This project is intended for educational purposes. Its monitoring results should be reviewed carefully and must not be treated as conclusive evidence of academic misconduct.
