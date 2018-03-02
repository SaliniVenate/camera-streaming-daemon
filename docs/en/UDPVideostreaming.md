# UDPVideoStreaming

[![Build Status](https://travis-ci.org/intel/camera-streaming-daemon.svg?branch=master)](https://travis-ci.org/intel/camera-streaming-daemon)
<a href="https://scan.coverity.com/projects/01org-camera-streaming-daemon">
  <img alt="Coverity Scan Build Status"
       src="https://scan.coverity.com/projects/12056/badge.svg"/>
</a>

UDP video streaming is currently supported only in gazebo. It requires gazebo enabled csd, QGC build from master.

1)Start the simulator: make posix gazebo_typhoon_h480
1)Open QGC select UDP Video Source in General Setting-> Video -> Video Source -> UDP Video Stream
2)Fill in UDP Port as 5600
3)Start the csd.(Note: In conf file of csd remove gazebo uri from uri section)
4)Fly the drone and observe the video in video area in fly view.
