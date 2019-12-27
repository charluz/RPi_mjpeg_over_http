# RPi_mjpeg_over_http
Practise MJPEG stream using RPi as the streamer server

MJPEG Stream Server on RPi: https://blog.csdn.net/xiao__run/article/details/76342634

# Quick Notes

## RPi
  1. sudo apt-get install libv4l-dev libjpeg-dev
  2. sudo apt-get install libjpeg9-dev
  
## MJPEG-STREAMER
  1. git clone https://github.com/jacksonliam/mjpg-streamer
  2. cd mjpg-streamer/mjpg-streamer-experimental/
  3. make clean && make all

## Start up MJpeg Stream
  $> ./mjpeg_streamer -i 'input_uvc.so -d /dev/video0' -o 'output_http.so -p 8080'
  
## Viewing stream on client PC
  http://IP:8080/?action=snapshot
  
 
