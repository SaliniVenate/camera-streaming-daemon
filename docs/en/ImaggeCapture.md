# ImageCapture 

[![Build Status](https://travis-ci.org/intel/camera-streaming-daemon.svg?branch=master)](https://travis-ci.org/intel/camera-streaming-daemon)
<a href="https://scan.coverity.com/projects/01org-camera-streaming-daemon">
  <img alt="Coverity Scan Build Status"
       src="https://scan.coverity.com/projects/12056/badge.svg"/>
</a>

Testing image capture requires mavlink enabled csd and a QGC app build from master.

1. Open QGC and disable the video streaming: General Settings->Video Source -> Video Stream Disabled.

2. Create a directory to store the image and update the location in imgcap section of conf file.

3. Now, in fly view of QGC app select camera mode and click on red button to take an image. The image will be stored in the location given in imgcap section in conf file.
