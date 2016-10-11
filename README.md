#NDVI algorithm for Raspberry Pi

This project provide several implementations of the NDVI real-time algorithm for Raspberry Pi and Raspberry Pi NoIR Camera.

**Note:**

	- All implementations assume that the Raspberry Pi and Pi NoIR Camera are properly configured.
	- This project is being tested with Raspberry Pi 3 and Pi NoIR Camera V1 Rev 1.3.

## Using Python algorithm:

Requirements:
  - Python 2.7 or higher;
  - OpenCV 2.4 or higher, can be installed in http://www.pyimagesearch.com/2016/04/18/install-guide-raspberry-pi-3-raspbian-jessie-opencv-3/;
	
Use:
  - Raspberry Pi open the terminal in this folder;
  - Run the command: `$ python Python/main.py`
  
## Using C++ algorithm:

Requirements:
  - RaspiCam: C++ API, version 1.3 or higher, can be installed in http://www.uco.es/investiga/grupos/ava/node/40;

Compile:
  - In C++ folder, run the command: `$ g++ main.cpp -o  main -I/usr/local/include/ -lraspicam -lraspicam_cv -lopencv_core -lopencv_highgui`

Use:
  - Raspberry Pi open the terminal in this folder;
  - Run the command: `$ ./C++/main`

## Benchmark
**Python:**
- 12 FPS;
- Resolution: 640x480;

**C++:**
- 20 FPS;
- Resolution: 640x480;
