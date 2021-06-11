# Install-OpenCV-Raspberry-Pi-64-bits
![output image]( https://qengineering.eu/images/LogoOpenRaspberryGitHub.webp )

## OpenCV installation script for a Raspberry Pi with 64-bits OS

[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)<br/>

This is the full setup of OpenCV for the Raspberry Pi 64-bits.<br/>
For more information see [Q-engineering - Install OpenCV Raspberry Pi](https://qengineering.eu/install-opencv-4.5-on-raspberry-64-os.html)

------------

## Installing OpenCV.
You must have allocated enough memory, otherwise the compilation, unfortunately, crashes after 2 hours at 100%
```
# check your total memory (RAM + swap) first. You need at least a total of:
# OpenCV 4.5.2 -> 6.5 GB!
# OpenCV 4.5.1 -> 5.5 GB
# OpenCV 4.5.0 -> 5.5 GB
# if not, enlarge your swap space as explained in the guide
$ free -m

$ wget https://github.com/Qengineering/Install-OpenCV-Raspberry-Pi-64-bits/raw/main/OpenCV-4-5-x.sh
$ sudo chmod 755 ./OpenCV-4-5-x.sh
$ ./OpenCV-4-5-x.sh
```
