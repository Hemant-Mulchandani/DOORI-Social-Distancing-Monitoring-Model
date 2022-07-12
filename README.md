# DOORI - Social Distancing Monitoring Model
A deep learning computer vision project built with OpenCV using YOLO(COCO model) object detector.

<h2> Motivation<span style='font-size:100px;'>&#127775;</span></h2>	
<p>
Social distancing is a method used to control the spread of contagious diseases. It implies that people physically distance themselves from one another, reducing close contact, and thereby reducing the spread of a contagious disease (such as the COVID-19 Disease). Social distancing is not a new concept, dating back to the fifth century, and has even been referenced in religious text such as the Bible.
</p>

<p align="center">
  <img src="Assets/social_distance_detector_spread.gif">
</p>

<p align="center">
   Social distancing plays crucial role in prevention of spread of Covid-19 virus.
</p>

## Features :gem:
* Object detection using the YOLO COCO model to detect only people in a video stream.
* Computes the pairwise distances between all detected people.
* Based on the computed distances, we determine whether social distancing rule is being violated or not.


## Installation :package:

1. Clone the repo

```bash
   $ git clone https://github.com/Hemant-Mulchandani/DOORI-Social-Distancing-Monitoring-Model.git
   $ cd social-distancing-detector
```

2. Install dependencies

```bash
   $ pip install -r requirements.txt
```

3. Run the main social distancing detector file. (set display to 1 if you want to see output video as processing occurs)
```bash
   $ python social_distancing_detector.py --input pedestrians.mp4 --output output.avi --display 0
```

## Usage :computer:
* Caution :bomb:\
For most accurate results, you should calibrate your camera through intrinsic/extrinsic parameters so that you can map pixels to measurable units.
An easier alternative(but less accurate) method would be to apply triangle similarity calibaration. Both of these methods can be used to map pixels to measurable units.\
If you do not want/cannot apply camera calibration, you can still utilize the social distancing detector but you'll have to rely strictly on the pixel distances, which won't necessarily be accurate.
For the sake of simplicity, this OpenCV Social Distancing detector implementation will rely on pixel distances. 
You can extend the implementation as you see fit though :wink:.

* YOLO COCO weights\
Github usually doesn't support files larger than 25 Mb.You can find the yolo weights in [My Google Drive](https://drive.google.com/file/d/1urxmtphDMakU9ffJEpIP-Ssi-_1djfc8/view?usp=sharing) or can be downloaded from <a href="https://pjreddie.com/media/files/yolov3.weights">here</a>.
Download weight file and add file to the yolo-coco folder.

* GPU\
Provided you already have OpenCV installed with NVIDIA GPU support, all you need to do is set ```USE_GPU=True``` in your ```config.py``` file.

## For CPU:

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

## For GPU:
You can find my google colab file here. [Social Distancing Detector Colab](https://colab.research.google.com/drive/1ZPBaO0w2qYR0TIj9L3kvQpwCegQom7u_?usp=sharing)

## Demo :movie_camera:

<p align="center">
  <img src="Assets/demo0.gif">
</p>

<p align="center">
  Raw Video as an input
</p>

#### After you run the last line of code or command, a window will pop up and after execution of the file a `output.avi` file will be showing up in your directory like this:

<p align="center">
  <img src="Assets/demo1.gif">
</p>

<p align="center">
  Processed Video as an output
</p>

## Want to talk more??

If you are interested in helping or have something to suggest or just want to chat with me, you can reach me through the following media .

- :e-mail: Email -mesg4hemant@gmail.com
- :pushpin: Let's connect on <a href="https://www.linkedin.com/in/Hemant-Mulchandani/">LinkedIn.</a> 

## References :book:
* Inspiration from Adrian Rosebrock's <a href="https://www.pyimagesearch.com/2020/06/01/opencv-social-distancing-detector/">OpenCV Social Distancing Detector</a> :heart:
* <a href="https://en.wikipedia.org/wiki/Social_distancing">Social Distancing</a>
* <a href="https://www.reddit.com/r/computervision/comments/gf4zhj/automatic_social_distance_measurement/">Automatic social distance measurement</a>
* <a href="https://www.linkedin.com/feed/update/urn%3Ali%3Aactivity%3A6661455400346492928/">Rohit Kumar Srivastava’s social distancing implementation</a>
* <a href="https://www.linkedin.com/feed/update/urn%3Ali%3Aactivity%3A6655464103798157312/">Venkatagiri Ramesh’s social distancing project</a>

## Todos :pencil:
* Utilize proper camera calibration.
* Apply top-down transformation of view angle.
* Improve the poeple detection process.

## License :key:
MIT &copy; License
