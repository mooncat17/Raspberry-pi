# Raspberry-pi
First pi
This is my first project from thoughts to implementaion 
There are many similar projects out there but they are not done by me. 
The goal of this project is not just complete the project, it is about the process.
There are so many free resources out there. However, it is sometimes confusing me as well. 
I try error and note it down here.

#Day01
Set up Raspberry Pi 3 (hardware)
1. power up - connect USB cable to Raspberry pi  
2. display setup  - connect HDMI cable to Rasbperry pi from TV
3. accessories setup  - connect usb extension hub to Rasbperry pi, Hub connects to mouse, keyboard 

Set up Rasbperry pi (software) 
My project needs to have audio output, and I want to use remotely access Pi 
So there are some setting have to be done before start programming.

[Set Time] -- will have alarm function

$date  #check current system time 
$systemctl status ntp
$ more /etc/ntp.conf | grep ^server 
$ sudo apt install ntpdate
$ sudo ntpdate -b -s -u ie.pool.ntp.org
$ sudo dpkg-reconfigure tzdata

