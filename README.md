# YoloFastest Jetson-Nano
![output image]( https://qengineering.eu/images/test_parkFV2.jpg )
## YoloFastest V2 with the ncnn framework. <br/>
[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)<br/><br/>
Special made for a bare Raspberry Pi 4, see [Q-engineering deep learning examples](https://qengineering.eu/deep-learning-examples-on-raspberry-32-64-os.html)

------------

## Benchmark.
| Model  | size | objects | mAP | Jetson Nano 2015 MHz | RPi 4 64-OS 1950 MHz |
| ------------- | :-----:  | :-----:  | :-----:  | :-------------:  | :-------------: |
| [NanoDet](https://github.com/Qengineering/NanoDet-ncnn-Raspberry-Pi-4) | 320x320 | 80 | 20.6  |  28.2 FPS | 13.0 FPS |
| [YoloFastestV2](https://github.com/Qengineering/YoloFastestV2-ncnn-Raspberry-Pi-4) | 352x352  | 80 | 24.1 |  **38.4 FPS** | 18.8 FPS |
| [YoloV2](https://github.com/Qengineering/YoloV2-ncnn-Raspberry-Pi-4) | 416x416  | 20 | 19.2 |  10.1 FPS | 3.0 FPS |
| [YoloV3](https://github.com/Qengineering/YoloV3-ncnn-Raspberry-Pi-4) | 352x352 tiny | 20 | 16.6 | 17.7 FPS | 4.4 FPS |
| [YoloV4](https://github.com/Qengineering/YoloV4-ncnn-Raspberry-Pi-4) | 416x416 tiny | 80 | 21.7 | 11.2 FPS | 3.4 FPS |
| [YoloV4](https://github.com/Qengineering/YoloV4-ncnn-Raspberry-Pi-4) | 608x608 full | 80 | 45.3 | 0.7 FPS | 0.2 FPS |
| [YoloV5](https://github.com/Qengineering/YoloV5-ncnn-Raspberry-Pi-4) | 640x640 small| 80 | 22.5 | 4.0 FPS | 1.6 FPS |
| [YoloX](https://github.com/Qengineering/YoloX-ncnn-Raspberry-Pi-4) | 416x416 nano | 80 | 25.8 | 17.6 FPS | 7.0 FPS |
| [YoloX](https://github.com/Qengineering/YoloX-ncnn-Raspberry-Pi-4) | 416x416 tiny | 80 | 32.8 | 8.3 FPS | 2.8 FPS |
| [YoloX](https://github.com/Qengineering/YoloX-ncnn-Raspberry-Pi-4) | 640x640 small | 80 | 40.5 | 2.6 FPS | 0.9 FPS |

------------

## Dependencies.
To run the application, you have to:
- The Tencent ncnn framework installed. [Install ncnn](https://qengineering.eu/install-ncnn-on-jetson-nano.html) <br/>
- OpenCV 64 bit installed. [Install OpenCV 4.5](https://qengineering.eu/install-opencv-4.5-on-raspberry-64-os.html) <br/>
- Code::Blocks installed. (```$ sudo apt-get install codeblocks```)

------------

## Installing the app.
To extract and run the network in Code::Blocks <br/>
$ mkdir *MyDir* <br/>
$ cd *MyDir* <br/>
$ wget https://github.com/Qengineering/YoloFastestV2-ncnn-Raspberry-Pi-4/archive/refs/heads/main.zip <br/>
$ unzip -j master.zip <br/>
Remove master.zip, LICENSE and README.md as they are no longer needed. <br/> 
$ rm master.zip <br/>
$ rm LICENSE <br/>
$ rm README.md <br/> <br/>
Your *MyDir* folder must now look like this: <br/> 
James.mp4 <br/>
parking.jpg <br/>
parking_tiny.jpg <br/>
YoloFastestV2.cpb <br/>
mainFV2.cpp <br/>
yolo-fastestv2.cpp <br/>
yolo-fastestv2.h <br/>
yolo-fastestv2-opt.bin <br/>
yolo-fastestv2-opt.param <br/>

------------

## Running the app.
To run the application load the project file YoloFastestV2.cbp in Code::Blocks. More info or<br/> 
if you want to connect a camera to the app, follow the instructions at [Hands-On](https://qengineering.eu/deep-learning-examples-on-raspberry-32-64-os.html#HandsOn).<br/><br/>
Many thanks to [dog-qiuqiu](https://github.com/dog-qiuqiu/Yolo-FastestV2) <br/><br/>
![output image]( https://qengineering.eu/images/Test_YoloF.jpg )<br/>
![output image]( https://qengineering.eu/images/Test_TFlite.jpg )<br/>
![output image]( https://qengineering.eu/images/Test_NanoDet.jpg )<br/>
![output image]( https://qengineering.eu/images/Test_MobileV1.jpg )

------------

[![paypal](https://qengineering.eu/images/TipJarSmall4.png)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=CPZTM5BB3FCYL) 