The images were found on the internet. I wrote the ruby code and the HTML file.

The entirety of the C code is licensed under the GPL.
The ruby and html files are licensed under the MIT license. A copy of the license is included with both files.

All the difficult C code was written by another author. The original contents of the file are below.

Real Time Eye Tracking and Blink Detection
==========================================

This project implements the algorithm (with small modifications) described in paper:

Real Time Eye Tracking and Blink Detection
Michael Chau and Margrit Betke
http://www.cs.bu.edu/techreports/pdf/2005-012-blink-detection.pdf

Overview
========

This system is the enhancement of my previous Eye Tracking system, where this system 
automatically locate the user's eye by detecting eye blinks. Motion analysis 
techniques are used in this stage, followed by online creation of the open eye template. 
The open eye template is used to locate the user's eye in the subsequent frames with 
template matching. Blink detection is performed using motion analysis techniques. 

Since the operation requires extensive amount of computation, the search region is 
restricted in a small search window around the user's eye. This method will drastically 
reduces the computation needed thus making the system running smoothly in real time.

Author:  Nashruddin Amin <me@nashruddin.com>
License: GPL
Website: http://nashruddin.com

See the complete tutorial at:
http://nashruddin.com/Real_Time_Eye_Tracking_and_Blink_Detection

Requirement
===========

This package requires the OpenCV library, freely available at:
http://sourceforge.net/projects/opencvlibrary

Compiling
=========

Compile as usual. See the OpenCV wiki (http://opencv.willowgarage.com) for info on how
to use various IDE with OpenCV.

Usage
=====
1. Run the program.
2. Blink your eyes. You will see 2 rectangles. The green rectangle labels
   the object being tracked (your eye) and the red rectangle is the search window.
3. Move your head to see the eye tracking.
4. If you blink, the program will display the text 'blink!' in the window.
5. Press 'r' to repeat eye detection.
6. Press 'q' to quit.

Contact the author
==================
Feel free to contact me@nashruddin.com.

