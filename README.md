# Emotion Detection Application

This repository contains the Emotion Detection application developed as the final project for the "Developing AI Applications with Python and Flask" course.

The application leverages the Watson NLP library to detect emotions (anger, disgust, fear, joy, and sadness) from user-provided text, packaged as an EmotionDetection module and deployed via a Flask web server.

## Project Structure

```text
oaqjp-final-project-emb-ai/
├── EmotionDetection/
│   ├── __init__.py
│   └── emotion_detection.py
├── static/
│   └── mywebscript.js
├── templates/
│   └── index.html
├── .gitignore
├── LICENSE
├── README.md
├── requirements.txt
├── server.py
├── test_emotion_detection.py
├── 6b_deployment_test.png
└── 7c_error_handling_interface.png
```

## Features

- **Emotion Detection Engine**: Utilizes Watson NLP Emotion Predict workflow to analyze text for five key emotions: anger, disgust, fear, joy, and sadness.
- **EmotionDetection Package**: Packaged module with clean interface for reusability.
- **Unit Testing**: Complete unit test suite (`test_emotion_detection.py`) covering positive, negative, and edge cases.
- **Web Interface**: Interactive web interface powered by Flask, Bootstrap, and JavaScript.
- **Robust Error Handling**: Handles blank inputs and error status codes (HTTP 400) gracefully.
- **Static Code Analysis**: High quality code with 10/10 score on Pylint.

## Installation & Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/sohamd530-eng/oaqjp-final-project-emb-ai.git
   cd oaqjp-final-project-emb-ai
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the application:
   ```bash
   python3 server.py
   ```

4. Access the web interface in your browser at `http://localhost:5000`.

## Running Unit Tests

Execute the unit tests using:
```bash
python3 test_emotion_detection.py
```

## Static Code Analysis

Run static code analysis using pylint:
```bash
pylint server.py
```
Expected score: `10.00/10`.
