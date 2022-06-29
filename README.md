***Winning project for WittyHacks 2.0 (central India's largest hackathon). Created by [Prathamesh Naik](https://github.com/neatpun), [Raghav Mahajan](https://github.com/Raghav-intrigue) & [Mohit Nathrani](https://github.com/Mohit-Nathrani).***
# Back-Off: Real Time Background Replacement
A tool that takes video and replace with new background provided by user in real time.

## Table of contents
- [Description](#description)
- [Technologies used](#technologies-used)
- [Results](#results)
- [How it works](#how-it-works)
- [Contributors](#contributors)


### Description
 Background removal helps with creative portrait photography and much more, helping provide the ability to change the background to a location of your choice. There are 4 methods available to use. One is a simple live-method using the webcam, a user can change the background by pressing and holding 'a', 'b', or 'c'. Other is live streaming from a mobile app. The last one is by requesting the server with pre-recorded video and background picture of choice. Fourth one is android app with a Flask server.
 
### Technologies Used
- Tensorflow
- OpenCV
- Flask

### Results
Input | Background | Result
:-------:|:---------:|:---------:
![input](images/a.jpg) | ![background](images/b.jpg) | ![output](images/c.jpg)

### How It Works
```sh
$ git clone https://github.com/neatpun/real-time-background-replacement
```

1. Live Webcam Front
* ```cd "Live Webcam Front" ``` 
* ```pip3 install -r requirements.txt```
* ```python live_webcam.py ```
* your code will just hang if you run this in GCP

2. Server Front
* ```cd "Server Front"```
* ```pip3 install -r requirements.txt```
* ```FLASK_APP=index.py flask run```
* then open localhost:5000 by clicking the hyperlink to it in your terminal
* provide video and background image
* after processing download of required video will begin

3. Live Stream Output
* ```cd "Live Stream Output"```
* ```pip3 install -r requirements.txt``` (have not created this file yet - not sure if we need it)
* connect any mobile device to same network and stream video.
* provide the ip address of mobile device in **IP_Webcam_Out.py**
* ```python IP_Webcam_Out.py```

4. Live Webcam in Flask App (test mode)
Accesses users webcam in the browers from a Flask App
* ```cd "Live Webcam App"```
* ---- Below is TODO ------
* ```pip3 install -r requirements.txt```
* ```FLASK_APP=app.py flask run```
* then open localhost:5000
* rest is TBD
* See the README file in the Live Webcam App for instructions to set up Google services