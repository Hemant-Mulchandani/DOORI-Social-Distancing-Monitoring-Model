# DOORI - Social Distancing Monitoring Model
A deep learning computer vision project built with OpenCV using YOLO(COCO model) object detector.

<h2> Motivation<span style='font-size:100px;'>&#127775;</span></h2>	
<p>
Social distancing is a method used to control the spread of contagious diseases. It implies that people physically distance themselves from one another, reducing close contact, and thereby reducing the spread of a contagious disease (such as the COVID-19 Disease). Social distancing is not a new concept, dating back to the fifth century, and has even been referenced in religious text such as the Bible.
</p>

<p align="center">
  <img src="Assets/social_distance_detector_spread.gif">
</p>

#### Github usually doesn't support files larger than 25 Mb.You can find the yolo weights in [My google drive](https://drive.google.com/file/d/1urxmtphDMakU9ffJEpIP-Ssi-_1djfc8/view?usp=sharing) 
* Download it & move to yolo-coco folder

# For CPU:

## To run this code in your terminal:
* ***Open your terminal**
* ***Change directory to where you have downloaded this code***
* ***Install python3 if you have not, if installed already then it's ok!***
* **Run**  `  python3 -m venv venv  ` ***to create a virtual environment named venv.***
* **Run**   `  source venv/bin/activate  ` 
***to activate your environment!***
* **Write**   `  pip install -r requirements.txt  ` 
***to install the python dependencies related to this project like opencv,numpy,scipy etc.***
* **Run the command** `time python social_distance_detector.py --input pedestrians.mp4 --output output.avi --display 1
` ***to run your social distance detection project***

#### After you run the last line of command,a window eill pop up and after execution of the file a `output.avi` file will be showing up in your directory like this:
![Output avi gif](https://github.com/abd-shoumik/Social-distance-detection/blob/master/social%20distance%20detection.gif)

# For GPU:
You can find my google colab file here. [Social Distancing Detector Colab](https://colab.research.google.com/drive/1ZPBaO0w2qYR0TIj9L3kvQpwCegQom7u_?usp=sharing)

## Contacts:
* **Created by: [Hemant Mulchandani](https://github.com/Hemant-Mulchandani)**
* **Email: mesg4hemant@gmail.com**
* **LinkedIn: [Hemant Mulchandani](https://www.linkedin.com/in/Hemant-Mulchandani/)**
