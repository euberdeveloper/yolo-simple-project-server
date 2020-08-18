# yolo-simple-project-client
The server part of a simple project made for a classmate

## Project purpose

I developed a project for another student of unitn. It is quite simple and consists in a frontend where the user selects a video, uploads it to a server. 
The servers uses yolo to recognize objects and sends back the resulted video, which is downloaded by the frontend.

## How was it made

The server is made with **python** because the used yolo libraries are for python. I used **Flask** for the api and also **gunicorn** to serve the flask application.

## How to run it

To run the frontend (Linux Ubuntu required):

* Install python 3 on your machine
* Clone this repo (`git clone https://github.com/euberdeveloper/yolo-simple-project-server.git`)
* Open the root folder in a terminal
* Execute `pip3 install -r requirements.txt` to install the python dependencies
* Execute `apt install libsm6 libxrender1 libfontconfig1 libice6` to install some needed apt dependencies for opencv
* Download from here [https://pjreddie.com/media/files/yolov3.weights](https://pjreddie.com/media/files/yolov3.weights) the yolov3 weights and put them in `/analyzer/weights/yolov3.weights`
* Execute `./run.sh` to start the server
* You can now make requests on the address 'http://localhost:5000'

The server is very very slow to process the video. If you need a bigger timeout, change the file `run.sh`, set the timeout in seconds after `--timeout`

## Demo

At this [link](https://yolo-simple-project-server.herokuapp.com) there is a demo hosted with Heroku. The problem is that the free Heroku plan does not have enough resources for our use of yolo, so only the image will work
