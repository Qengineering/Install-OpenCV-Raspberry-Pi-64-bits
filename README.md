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
# OpenCV 4.5.4 -> 6.5 GB!
# OpenCV 4.5.3 -> 6.5 GB!
# OpenCV 4.5.2 -> 6.5 GB!
# OpenCV 4.5.1 -> 5.5 GB
# OpenCV 4.5.0 -> 5.5 GB
# if not, enlarge your swap space as explained in the guide
$ free -m

$ wget https://github.com/Qengineering/Install-OpenCV-Raspberry-Pi-64-bits/raw/main/OpenCV-4-5-x.sh
$ sudo chmod 755 ./OpenCV-4-5-x.sh
$ ./OpenCV-4-5-x.sh
```
:point_right: Don't forget to reset your swap memory afterwards.

------------

If you want to beautify OpenCV with the Qt5 GUI you need to
- $ sudo apt-get install qt5-default
- Set the -D WITH_QT=**ON** \ (± line 54) in the script<br/>
 
before running the script on your RPi

------------

OpenCV will be installed to the `/usr/local` directory, all files will be copied to following locations:<br/>

- `/usr/local/bin` - executable files<br/>
- `/usr/local/lib` - libraries (.so)<br/>
- `/usr/local/lib/cmake/opencv4` - cmake package<br/>
- `/usr/local/include/opencv4` - headers<br/>
- `/usr/local/share/opencv4` - other files (e.g. trained cascades in XML format)<br/>
