# FaceTrack- Facial Attendance System
FaceTrack - an AI-Based Facial Attendance System developed in 1 day for the T-Hunt Hackathon conducted by the School of Computer Science, Manipal University Jaipur. 

## Demo Video

Here is a video demonstrating our system i.e. our Web App:

https://user-images.githubusercontent.com/53339132/213921247-3f46411a-23b7-4f6d-862d-0922ce733e56.mp4

## Prerequisites to deploy and use the Web App
  - **Python** should be installed on the system to run the Backend of the Web App.
  - **Pip** should be installed on the system to install dependencies of the Back End of the Web App.
  - The following packages should be installed by using pip on the system (run the following commands in Command Prompt/Terminal after installing python and pip to install them):
    
    ```bash
    pip install tornado
    pip install opencv-python
    pip install numpy
    pip install Pillow
    ```

## Instructions to deploy and use the Web App
  - Download the project and extract the files in any folder.
  - Open Command Prompt/Terminal and navigate to the **"Backend"** folder.
  - In the **"Backend"** folder, run the **"app.py"** file to start the Facial Recognizer AI WebSocket Server by running the following command:
    
    ```bash
    python app.py
    ```
    
  - Then, open a new instance of the Command Prompt/Terminal and navigate to the **"Frontend"** folder.
  - Run the following command in the **"Frontend"** directory to start the Frontend HTTP Server:
    
    ```bash
    python -m http.server 5000
    ```
    
    Note: here 5000 is the port at which the HTTP Server will run and you could set it to anything you want.
  
  - Done! The Web App is now deployed and can be accessed at **http://localhost:5000** (replace 5000 with the port which you used in the previous command).
  - In the Web App, first, go to the Register page to register yourself in the System.
  - Then, go to the Mark Attendance page to mark your attendance for the day.

## Limitations of the project

 - Since the whole project was developed on a Laptop, the training capabilities of the model were restricted, and hence is trained using merely 100 images per student which is pretty low as compared to the standard training requirement.
 - Even then it has a fairly high accuracy. But due to a lack of proper model training, it can confuse between students and identify them incorrectly.
 - Due to restricted computing power, it can take longer than usual by the model recognizer to recognize a student.
 - We will overcome and fix these limitations in the near future, once we get the resources needed to do the proper model training and faster recognition.

## Team

1. **Nikhil Dixit ([@nikdixit](https://github.com/nikhildixit27))** : Responsible for the Frontend of the web app.
2. **Abhay Tripathi ([@abhaytr](https://github.com/abhaytr))** : Responsible for the Backend of the web app.
