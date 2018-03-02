# CameraControl

[![Build Status](https://travis-ci.org/intel/camera-streaming-daemon.svg?branch=master)](https://travis-ci.org/intel/camera-streaming-daemon)
<a href="https://scan.coverity.com/projects/01org-camera-streaming-daemon">
  <img alt="Coverity Scan Build Status"
       src="https://scan.coverity.com/projects/12056/badge.svg"/>
</a>

Testing camera control parameters requires mavlink enabled csd, a QGC app build from master and a http server (Follow https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-on-ubuntu-16-04 to install apache server).

1. Host the camera definition file present in samples directory using http server. To host using apache server copy the file to /var/www/html:

    $ cp ~/camera-streaming-daemon/samples/camera-def-rs-rgb.xml /var/www/html

The aero image has an aero-http server to host camera definition file. Copying the camera defenition files to /var/http will host the files.

2. Update the uri section in conf file with appropriate ip adress. Sample conf files are present in files folder in samples directory.

3. Open QGC build from master. Select General Settings->Video Source -> RTSP Video Stream. Fill in the video uri and observe the video in fly view.

4. In fly view, select camera from dropdown list located in top right corner under compass. Settings button in left top corner of the box can be used to set the control parameters of the camera.

