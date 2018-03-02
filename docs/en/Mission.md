# ImageCapture 

[![Build Status](https://travis-ci.org/intel/camera-streaming-daemon.svg?branch=master)](https://travis-ci.org/intel/camera-streaming-daemon)
<a href="https://scan.coverity.com/projects/01org-camera-streaming-daemon">
  <img alt="Coverity Scan Build Status"
       src="https://scan.coverity.com/projects/12056/badge.svg"/>
</a>

Testing image capture while executing a mission requires mavlink enabled csd and a QGC app build from master.

1) Create a directory to store the image and update the location in imgcap section of conf file.
3) Open QGC and switch to Plan View.
4) Create a mission using available plan tools.
5) Edit the mission: At required waypoints choose "Take photo" from dropdown list under camera.
6) Send the mission to the vehicle.
7) Change to Fly View and fly the mission.
8) The captured images will be stored in the location given in imgcap section in conf file.
