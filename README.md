# AI Sign Language Recognition System

An AI-powered American Sign Language (ASL) alphabet recognition system that uses computer vision and machine learning to recognize hand gestures through a webcam and convert them into readable text.

## Project Overview

The **AI Sign Language Recognition System** is designed to help bridge communication gaps between people who use sign language and those who may not understand it.

The system detects hand gestures using a webcam, extracts hand landmarks with MediaPipe, and uses a trained machine learning model to predict the corresponding ASL alphabet letter.

Recognized letters can be combined to form words and text.

## Objectives

- Recognize American Sign Language alphabet gestures.
- Detect and track hand landmarks using MediaPipe.
- Train and evaluate machine learning classification models.
- Recognize hand gestures through a live webcam.
- Convert recognized letters into readable text.
- Provide an interactive interface for testing the system.

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| Google Colab | Development and experimentation |
| OpenCV | Image processing |
| MediaPipe | Hand landmark detection |
| NumPy | Numerical operations |
| Pandas | Data handling |
| Scikit-learn | Machine learning models |
| Gradio | Webcam interface |
| Matplotlib | Data visualization |

## How It Works

1. **Image Input:** The system receives hand gesture images or webcam frames.
2. **Hand Detection:** MediaPipe detects the hand and identifies 21 hand landmarks.
3. **Feature Extraction:** The landmark coordinates are normalized and converted into numerical features.
4. **Model Prediction:** A trained machine learning classifier predicts the corresponding ASL letter.
5. **Text Formation:** Stable predictions are combined to form readable text.

## Machine Learning Approach

The project uses hand landmark coordinates rather than relying only on raw image pixels.

- 21 hand landmarks are extracted.
- Each landmark contains X, Y, and Z coordinates.
- A total of 63 numerical features are generated per detected hand.
- Features are used to train and evaluate classification models.
- Random Forest and Support Vector Machine (SVM) models are explored.

## Dataset

The project uses the ASL Alphabet dataset from Kaggle.

Dataset: [ASL Alphabet Dataset – Kaggle](https://www.kaggle.com/datasets/grassknoted/asl-alphabet)

The dataset contains images representing ASL alphabet signs and additional classes. The implemented experiments focus on the classes selected for model training.

**Note:** The dataset itself is not included in this repository. Download it separately from Kaggle.

## Main Features

- Hand landmark detection.
- ASL alphabet classification.
- Machine learning model experimentation.
- Live webcam recognition.
- Prediction confidence/relative score display.
- Stable gesture detection.
- Letter-to-text formation.
- Interactive Gradio interface.

## Project Structure

A recommended repository structure is:

```text
ai-sign-language-recognition-system/
│
├── notebooks/
│   └── asl_sign_language_recognition.ipynb
│
├── src/
│   ├── feature_extraction.py
│   ├── model_training.py
│   └── prediction.py
│
├── app/
│   └── webcam_app.py
│
├── models/
│   └── README.md
│
├── reports/
│   └── project_report.pdf
│
├── requirements.txt
├── .gitignore
└── README.md
```

Adjust this structure to match the actual files included in the project.

## Installation

Clone the repository:

```bash
git clone https://github.com/HAMID12344/ai-sign-language-recognition-system.git
```

Move into the project directory:

```bash
cd ai-sign-language-recognition-system
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Open the notebook in Google Colab or Jupyter Notebook and follow the project workflow.

## Running the Project

The project can be explored through its Jupyter notebook.

The webcam application can be launched using the Gradio interface code after the required model and dependencies have been loaded.

## Evaluation

The project includes model experimentation, dataset evaluation, and webcam-based testing.

Performance results should be reported separately for each model and test method. Dataset accuracy should not be treated as live webcam accuracy.

## Current Project Scope

The current implementation focuses on static ASL alphabet recognition.

Full dynamic sign recognition, facial expressions, sign-language grammar, and complete sentence translation are outside the initial project scope.

## Future Improvements

- Improve recognition under different lighting conditions.
- Expand testing with independent webcam images.
- Support more hand gestures.
- Explore dynamic sign recognition.
- Add text-to-speech functionality.
- Develop a more advanced user interface.

## Project Information

**Project Title:** AI Sign Language Recognition System

**Subtitle:** A Computer Vision-Based Hand Gesture to Text Application

**University:** Bahria University, Islamabad Campus

**Department:** Department of Computer Sciences

**Program:** BS Information Technology (BSIT)

**Course:** Artificial Intelligence

**Instructor:** Ms. Farwa Kazmi

**Project Members:**
- Hamid Ali
- Hassan Mehmod

## Acknowledgements

We acknowledge the creators of the ASL Alphabet dataset and the developers of the open-source libraries used in this project.

---

**Developed as an academic project for the Artificial Intelligence course at Bahria University.**
