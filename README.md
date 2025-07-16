# Face Recognition Attendance System


## Introduction

This Python-based system utilizes face recognition technology to automate attendance tracking. It features a user-friendly graphical interface (GUI) built with Tkinter, enabling efficient student registration, real-time attendance marking via webcam, and comprehensive attendance record viewing. This solution is designed to streamline attendance management in educational and organizational environments.

## System Requirements

This project relies on the following Python libraries:

*   `numpy`
*   `opencv-contrib-python`
*   `opencv-python`
*   `openpyxl`
*   `pandas`
*   `Pillow`
*   `pyttsx3`

## Setup and Installation Guide

To set up and run the project, please follow these steps:

1.  **Obtain the Repository:** Clone or download this repository to your local machine.
2.  **Install Dependencies:** Navigate to the project's root directory in your command prompt or terminal and execute the following command to install all necessary packages:
    ```bash
    pip install -r requirements.txt
    ```
3.  **Create Training Directory:** Create a folder named `TrainingImage` within the project's root directory. This folder will store the captured facial images.
4.  **Update File Paths:** Open `attendance.py` and `automaticAttedance.py`. Update all file paths within these scripts to reflect your system's directory structure.
5.  **Launch Application:** Execute the `attendance.py` file to start the application.

## Project Workflow and Functionality

Upon launching the application, the primary workflow involves registering individuals, training the recognition model, and then utilizing it for attendance tracking.

1.  **Student Registration:**
    *   Click the "Register new student" button.
    *   A new window will appear, prompting for the student's ID and name.
    *   Click "Take Image." A camera feed will activate, detecting the face and capturing up to 50 images (this quantity is configurable). These images are stored in the `TrainingImage` folder. Capturing a higher number of diverse images will enhance recognition accuracy.
    *   Subsequently, click "Train Image." This process trains the facial recognition model by converting the captured images into a numerical format that the system can interpret. This step is crucial for enabling the system to identify faces accurately in subsequent operations. The duration of this process will vary depending on your system's specifications.

2.  **Automatic Attendance:**
    *   After the model is trained, click "Take Attendance."
    *   Enter the subject name for which attendance is to be recorded.
    *   The system will activate the webcam, recognize enrolled faces, and automatically mark attendance.
    *   Attendance records are saved as `.csv` files, with a separate file generated for each subject.

3.  **View Attendance:**
    *   Click the "View Attendance" button.
    *   Enter the desired subject name.
    *   The attendance record for that subject will be displayed in a tabular format.

 
## Project Snapshots:

*   **Simple UI:**
*   ![Simple UI](UI_Image/simple_ui.png) 
*   **While taking Image:**
*    ![While taking Image](UI_Image/simple_ui.png) 
*   **While taking Attendance:**
*    ![While taking Attendance](UI_Image/simple_ui.png) 
*   **Attendance in tabular format:**
*    ![Attendance in tabular format](UI_Image/simple_ui.png) 

 

## **Support the Project:  Your support is highly appreciated! Please consider starring ⭐ this repository.**
