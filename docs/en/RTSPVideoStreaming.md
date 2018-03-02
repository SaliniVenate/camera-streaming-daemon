# VideoStreaming

[![Build Status](https://travis-ci.org/intel/camera-streaming-daemon.svg?branch=master)](https://travis-ci.org/intel/camera-streaming-daemon)
<a href="https://scan.coverity.com/projects/01org-camera-streaming-daemon">
  <img alt="Coverity Scan Build Status"
       src="https://scan.coverity.com/projects/12056/badge.svg"/>
</a>

Testing of RTSP  video streaming can be done using a vlc player or a gstreamer client pipeline or a QGroundcontrol app.

To test video streaming using vlc:

$ vlc rtsp://<ip_csd_running_system>:8554/<videox>

To test video streaming using gstreamer client pipeline:

$ gst-launch-1.0 uridecodebin uri=<ip_csd_running_system>:8554/<videox> ! autovideosink

In order to test the video streaming using QGC, select RTSP Video Source in General Setting-> Video ->Video Source and fill in uri as rtsp://ip_csd_running_system:8554/<videox>. Observe the video in video area in fly view.
