**Face Detetction Using NVIDIA VILA and Face Dataset**

This project demonstrates a simple, interactive web application for face detection and image description using NVIDIA's VILA Vision-Language Model API. It focuses on extracting face images from the popular Labeled Faces in the Wild (LFW) dataset and allows users to either select a sample face or upload their own custom image for automated semantic description.

**Features**

Face Selection: Choose sample images from the LFW dataset or upload your own photo.

Semantic Image Description: Sends the selected/uploaded image to the NVIDIA VILA API, which generates a detailed, human-readable description of the scene or face.

Web Interface: Available in both Streamlit and Gradio implementations, enabling easy use and sharing.

Image Preprocessing: Handles grayscale to RGB conversions and prepares images for API requests.

**Technologies Used**

1) Python

2) Streamlit and Gradio for frontend web/app development

3) PIL, NumPy, and scikit-learn for image processing and dataset handling

4) NVIDIA VILA API for deep learning-based vision-language inference

**How it Works**

Select or Upload Image: The app provides options to choose faces from the LFW dataset or upload a custom image.

API Request: The chosen image is encoded in base64 and sent in a prompt to the NVIDIA VILA API.

Result Display: The API returns a semantic description, which is then displayed to the user.

**Sample Usage**

Run the app using Streamlit:

streamlit run app.py

Or launch the Gradio interface (example code included in the repository).

**Example Output**

Given a close-up portrait of a well-known personality, the app might return:

"The image is a black and white portrait of [given person], with a serious expression, looking off to the side. The background is blurred, drawing attention to the face. The monochrome color scheme adds a timeless quality to the portrait."

**Installation**

1) Clone the repository

2) Install required Python packages:
    pip install streamlit gradio scikit-learn pillow numpy requests
3) Run locally (or use public URL sharing via Gradio or Streamlit as demonstrated in the notebook).

**Credits**

Uses the Labeled Faces in the Wild dataset (scikit-learn)

Powered by NVIDIA VILA Vision-Language Model API

This project helps demonstrate the practical integration of computer vision, machine learning APIs, and modern Python web frameworks for intelligent, interactive applications.
