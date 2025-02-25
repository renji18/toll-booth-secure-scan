
# Toll Booth Number Plate Scanner Project

The Toll Booth Number Plate Scanner Project is a Python based application designed to handle the processing, storage, and retrieval of number platedata from a car as soon as it stops near the toll booth. It provides functionality for uploading number plate files, processing them, and filtering the data from a database.

## Installation

Follow these steps to install and set up the project:


1. Clone the repository:

   ```bash
   git clone [https://github.com/your-username/your-project.git](https://github.com/renji18/toll-booth-secure-scan.git)
   cd your-project

2. Set up a virtual environment (optional but recommended):

    ```bash
    python -m venv venv
    source venv/bin/activate

3. Install the dependencies:

    ```bash
    pip install -r requirements.txt

4. Start the application:

    ```bash
    python main.py


## Usage

### Uploading Data
1. Start the application by running `python main.py`

2. Once the camera is up and running, place a sample image of a car with numberplate in front of your camera.

3. Once the camera is able to recognize the number plate, press `s` on your keyboard, you'll have the number plate as an output in your terminal.


## Dependencies
The project relies on the following Python packages:

```easyocr```
```opencv-python```

You can install these dependencies using `pip install -r requirements.txt`.


## Project Report


1. Project Overview:
The project is a Python-based application designed for real-time detection and recognition of vehicle number plates using computer vision and optical character recognition (OCR) techniques. The primary goal is to develop a system that can process live video feed from a camera, detect license plates, and extract the text information from them using the EasyOCR library.


2. Problem Statement:
The project addresses the need for an efficient and automated solution for vehicle license plate recognition. Manual extraction of information from license plates can be time-consuming and error-prone. This project aims to automate this process, providing a faster and more accurate method for retrieving license plate data.


3. Solution Overview:
The solution involves the integration of computer vision and OCR technologies to identify and extract license plate information. The key components of the solution include:

OpenCV for Computer Vision:
The project utilizes the OpenCV library for computer vision tasks. It captures video frames from a camera, converts them to grayscale, and applies a cascade classifier to detect potential license plates.

EasyOCR for Optical Character Recognition:
The EasyOCR library is employed to perform OCR on the region of interest (ROI) containing the license plate. It recognizes and extracts the alphanumeric characters from the license plate image.

Real-time Processing:
The application is designed to process video frames in real-time, allowing for continuous monitoring of the camera feed. This is achieved through a loop that captures frames, detects license plates, and extracts information.


4. Code Explanation:
The main.py script contains the main logic of the application. Here's a breakdown of the code:

Initialization:
The script initializes the EasyOCR reader and sets up the video capture using OpenCV. It also configures the minimum area for license plate detection.

Frame Processing Loop:
The core of the script is a continuous loop that captures video frames, applies license plate detection, and performs OCR on the detected plates. If a key is pressed (in this case, 's'), it triggers OCR on the region of interest (ROI) and prints the recognized text.

License Plate Detection:
License plate detection is performed using OpenCV's cascade classifier. The script iterates through the detected plates, and if the area exceeds a predefined threshold, it highlights the plate on the frame.

OCR and Output:
The OCR process is triggered when the 's' key is pressed. The recognized text is then printed to the console. Additional functionality, such as saving images or displaying results on the frame, is commented out but can be enabled based on project requirements.

s
5. Future Scope:
The project has several avenues for future improvement and expansion:

Enhanced Accuracy:
Fine-tune the OCR and detection algorithms to improve accuracy, especially in challenging lighting and environmental conditions.

Database Integration:
Implement a database to store and manage recognized license plate information for historical and analytical purposes.

Web Interface:
Develop a web-based interface to visualize and interact with the recognition results, enabling users to search, filter, and export data.

Multiple Camera Support:
Extend the system to support multiple cameras simultaneously, enhancing its usability in larger-scale scenarios.

Cloud Integration:
Explore the integration of cloud services for storage, processing, and analysis, enabling scalable and distributed solutions.

By addressing these future scopes, the project can evolve into a comprehensive and versatile solution for license plate recognition with broader applications.