
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

3. Start the application:

    ```bash
    python app.py


## Usage

### Uploading Data
1. Start the application by running `python app.py`

2. Once the camera is up and running, place a sample image of a car with numberplate in front of your camera.

3. Once the camera is able to recognize the number plate, press `s` on your keyboard, you'll have the number plate as an output in your terminal.


## Dependencies
The project relies on the following Python packages:

```easyocr```
```opencv-python```

You can install these dependencies using pip install -r requirements.txt.
