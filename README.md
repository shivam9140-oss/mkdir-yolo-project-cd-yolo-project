🚀 YOLO Object Detection Project
This project implements YOLO (You Only Look Once), a real-time object detection system, to detect various objects through a webcam. Using the YOLO model, this program can detect objects like people, vehicles, animals, and more in real-time as the camera captures the video feed.

🧑‍💻 How It Works:
The program uses a pre-trained YOLO model to recognize objects in real-time.

The webcam captures live video, and YOLO processes each frame to identify objects.

Bounding boxes and confidence scores are drawn around detected objects.

The system runs at high speeds with live FPS (Frames Per Second) calculation, displaying the performance in real-time.

The program stops when you press the q key.
🔧 Project Requirements:
To run this project, you need to install a few Python dependencies. You can install them using requirements.txt:

📝 Install Dependencies:
pip install -r requirements.txt
Or, you can manually install the required libraries:

bash
Copy code
pip install ultralytics opencv-python cvzone
Ultralytics: The library used for YOLO implementation.

OpenCV: For video capture and image processing.

CVZone: Used for drawing bounding boxes and displaying text.

🛠 How to Run the Project:
Ensure you have the YOLO weights file (such as yolo12s.pt) available. You can download pre-trained YOLO models from the official YOLO website.

Clone the repository or download the project files to your computer.

Open a terminal or command prompt, navigate to the project directory, and run:

bash
Copy code
python main.py
The webcam will open, and real-time object detection will begin. The detected objects will be highlighted with bounding boxes.

Press q to stop the program.

🔑 YOLO Model Path:
Make sure to provide the correct path to your YOLO model. By default, the model is loaded from:

python
Copy code
model = YOLO("path/to/your/yolo12s.pt")  # Correct path to your model file
If your model file is in a different location, modify this line accordingly.

🧑‍🎓 Supported Objects:
The YOLO model detects a variety of objects based on the COCO dataset. Some of the detected objects include:

People (person, dog, cat, etc.)

Vehicles (car, bus, motorbike, etc.)

Animals (sheep, cow, elephant, zebra, etc.)

Everyday Items (bottle, laptop, chair, etc.)

Here is a partial list of detected objects:

Person

Bicycle

Car

Dog

Cat

Laptop

Chair

Book

... and many more!

📸 Demo:
When you run the code, you will see a live feed from your webcam with bounding boxes drawn around the detected objects. The confidence score and the object class name are displayed on the screen.

📍 Project Folder Structure:
The project folder will look like this:

graphql
Copy code
yolo-project/
├── main.py        # The main code file with YOLO implementation
├── README.md      # Project description and instructions
├── requirements.txt  # List of required Python libraries (optional)
└── yolo12s.pt     # YOLO model weights (make sure to download or place it correctly)
⚡ Performance:
This program calculates the FPS (frames per second) of the video feed, ensuring smooth real-time detection. FPS is displayed in the top-left corner.

🎉 Enjoy Using YOLO for Object Detection!

