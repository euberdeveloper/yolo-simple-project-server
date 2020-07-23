# yolo-simple-project-client
The client part of a simple project made for a classmate

# Project purpose

I developed a project for another student of unitn. It is quite simple and consists in a frontend where the user selects a video, uploads it to a server. 
The servers uses yolo to recognize objects and sends back the resulted video, which is downloaded by the frontend.

# How was it made

The frontend is made with Vue.js and a Node.js to serve it. I used the VueSax UI library and axios for the requests. I also used typescript with Vuejs in order to have a cleaner code.

# How to run it

To run the frontend:

* Install nodejs on your machine
* Clone this repo (`git clone https://github.com/euberdeveloper/yolo-simple-project-client.git`)
* Open the root folder in a terminal
* Execute `npm run frontend:install` (an alternative could be `cd vuejs && npm install`) to install the frontend dependencies
* Execute `npm install` to install the nodejs server dependencies
* Execute `npm run frontend:build` (an alternative could be `cd vuejs && npm run build`) to build the frontend
* Execute `npm start` to start the frontend server
* You can now open your browser on the address 'http://localhost:8000'

# Demo

At this [link](https://yolo-simple-project-client.herokuapp.com) there is a demo hosted with Heroku. The problem is that the free Heroku plan does not have enough resources for our use of yolo, so only the image will work
