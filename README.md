# raspberry-monitor
Simple gstreamer configuration to stream from a raspberry pi

You first need to add 
boot_delay=1
start_x=1
gpu_mem=128
to /boot/config.txt

You need to install gstreamer and its dev components
sudo apt install gstreamer1.0-tools libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev

And install gst-rpicamsrc
https://github.com/thaytan/gst-rpicamsrc

stream-video.service and stream-audio.service goes to /etc/systemd/system/
stream-video and stream-audio goes to /etc/default/ and should be edited to match the host ip and listening port
