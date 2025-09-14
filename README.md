# Multi-Channel Digital Arrest Fraud Scam Detection

This project is a multi-channel scam detection system that analyzes text, audio, and video inputs to identify potential frauds and scams, with a focus on "digital arrest" scams.

-----

## Features

  - **Text Analysis**: Detects scams from text messages, emails, etc., by identifying risky keywords.
  - **Audio Analysis**: Transcribes audio and analyzes the text for scam-related content.
  - **Video Analysis**: Analyzes video files by extracting audio and examining frames for deepfakes.
  - **Real-Time Alerts**: Provides real-time alerts through a web interface when a scam is detected.

-----

## How it works

The system uses a combination of machine learning models to analyze different types of inputs:

  - A **Text Classifier** model is used to predict whether a given text is a scam or not.
  - An **Audio Processor** model transcribes audio files into text, which is then fed into the text classifier.
  - A **Video Deepfake Detector** analyzes video frames to detect deepfakes.

The project uses a **FastAPI** backend to handle the analysis requests and a **WebSocket** connection to send real-time alerts to the frontend.

-----

## How to use

1.  **Clone the repository**:
    ```bash
    git clone https://github.com/learnwithyourself2525-create/multi-channel-digital-arrest-fraud-scam-detection.git
    ```
2.  **Run the backend**:
    The backend is a FastAPI application. To run it, you need to have Python and the required packages installed.
3.  **Open the web interface**:
    Open the `index.html` file in the `ui/templates` directory in your web browser to interact with the system.

You can then use the web interface to analyze text, audio, and video files for potential scams.

-----

## Project Structure

  - `alerts/`: Contains the code for managing real-time alerts.
  - `data/`: Contains the datasets used for training the models.
  - `models/`: Contains the machine learning models for text, audio, and video analysis.
  - `pipeline/`: Contains the detection pipeline that processes the inputs and runs them through the models.
  - `ui/`: Contains the frontend code for the web interface.
  - `utils/`: Contains utility functions.
