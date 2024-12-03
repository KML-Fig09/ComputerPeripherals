# Pilot Project: YOLOv5 Computer Peripherals Object Detection

**This pilot project develops a YOLOv5 Object Detection model for detecting computer peripherals in Twitch streams. The successes and failures of this project contribute extensively to the progress of an advanced YOLOv5 model, with custom CBAM module, created as a final project contributing to my Master of Science. Though this project earned a distinction, there's plenty to improve on too. The primary issue with this model was the data, or lack thereof, it was trained on. Additionally, a lack of vision regardings steps which were applied afterwards. These are handled in the final project, also found on this Github, by preprocessing, combining, and augmenting 7 different Roboflow datasets for training - as well as developing a tracking (Norfair) and Segmentation (SAM) pipeline post-detections. 

This repository contains the Jupyter Notebook titled **"YOLOV5_ObjectDetection.ipynb"**. This notebook was developed in **Google Colab** and is intended to be run within that environment.

## Contents

1. Notebook including model etc.
2. Test video for inference (creator acknowleged in this README)
3. This README.
4. requirements.txt file.

## Overview

The notebook includes a series of data analysis tasks that require specific libraries and configurations, which are pre-installed and configured in Google Colab. It is highly recommended to use Google Colab for running this notebook to avoid dependency and environment issues.

## Running the Notebook in Google Colab

To run this notebook in Google Colab:

1. Upload the notebook to your Google Drive.
2. Open it with Google Colab by right-clicking the file and selecting "Open with" -> "Google Colab".
3. All necessary libraries and dependencies should be pre-installed. If any additional installations are required, they are handled within the notebook itself.

## Running the Notebook in Other Environments

If you prefer to run this notebook in a different environment (e.g., Jupyter Notebook locally), here are some steps you may need to follow:

1. **Clone the Repository**: Clone this repository to your local machine using:
    ```sh
    git clone https://github.com/KML-Fig09/Yolov5-CBAM-Object-Detection.git
    ```

2. **Install Required Libraries**: You will need to manually install the required Python libraries. Create a virtual environment and install the dependencies using the following commands:
    ```sh
    python3 -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`
    pip install -r requirements.txt  # If a requirements.txt file is provided
    ```
    Alternatively, if no `requirements.txt` is provided, you may need to install libraries such as:
    ```sh
    pip install numpy pandas matplotlib seaborn scikit-learn
    ```

3. **Run the Notebook**: Start Jupyter Notebook in the terminal:
    ```sh
    jupyter notebook
    ```
    Then, open the notebook file `YOLOV5_ObjectDetection` from the Jupyter Notebook dashboard.

4. **Adjustments**: Depending on your local setup, you may need to adjust file paths or install additional dependencies that are not included in the notebook.

## Troubleshooting

- **Dependency Issues**: If you encounter any dependency issues or missing libraries, refer to the error messages and install the required packages using `pip install <package-name>`.
- **Environment Issues**: The notebook is designed for Colab, which has many libraries pre-installed. If running locally, you may need to manually install more libraries or adjust some code blocks.

## Contributing

Feel free to submit a pull request or open an issue if you find any bugs or have suggestions for improvements.

## Acknowlegments 

icyJL, 2024. Valorant RANK 1 Radiant Setup Tour. [Online Video]. Available at: 
https://www.youtube.com/watch?v=zMl2Rie4SDc&t=22s [Accessed June 05, 2024]. 

Roboflow (2024) Raava Dataset. Available at: https://universe.roboflow.com/mouse
2lugf/raava/dataset/1 (Accessed: 01 June 2024) 
