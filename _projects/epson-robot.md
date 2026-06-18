---

layout: project
title: "Epson Cargo Storing Robot"
description: "Autonomous cargo storing system using Epson T3-401S and computer vision."
permalink: /projects/epson-robot/

categories:

* Robotics
* Mechatronics

project_folder: "epson-robot"
featured_image: "/assets/projects/epson-robot/cover.png"

models:

* file: "/assets/projects/epson-robot/epson-adapter.glb"
  description: "Custom Epson T3 Adapter"

* file: "/assets/projects/epson-robot/gripper.glb"
  description: "3D Printed Servo Gripper"

media:

* file: "cover.png"
  title: "The System"
  description: "Epson cargo storing system."

* file: "system-diagram.png"
  title: "System Architecture"
  description: "Overall system architecture."

* file: "image1.jpeg"
  title: "Robot Setup"
  description: "Testing and calibration of the Epson T3-401S robot."

* file: "demo-video.mp4"
  title: "Project Demonstration"
  description: "Full autonomous cargo storing operation."

download_files:

* name: "Complete Source Code"
  url: "/assets/projects/epson-robot/source-code.zip"
  description: "Python, Epson RC+ and Arduino source code."

---

## Overview

Autonomous cargo storing system using an Epson T3-401S SCARA robot and an ESP32-CAM vision system. The system uses computer vision and industrial robotics to detect cargo positions, calculate coordinates, and automatically perform pick-and-place operations.

## Features

* ArUco marker detection
* OpenCV-based computer vision
* TCP/IP communication between Python and Epson RC+
* Automatic cargo storing
* Real-time coordinate conversion
* Custom 3D-printed gripper
* Custom Epson T3 adapter
* Arduino-controlled servo gripper
* Industrial SCARA robot integration

## System Architecture

The system consists of an ESP32-CAM for image acquisition, a Python/OpenCV vision system for object detection and coordinate calculation, an Epson RC+ controller for robot motion planning, and a custom servo gripper for cargo handling.

## Code Overview

### Python / OpenCV

The Python code receives the ESP32-CAM video stream, detects ArUco markers, calculates object coordinates, and sends the position data to the Epson robot controller.

### Epson RC+

The Epson RC+ program receives coordinates from Python and controls the Epson T3-401S robot to perform the pick-and-place operation.

### Arduino

The Arduino Uno controls the servo gripper, handling opening and closing actions during the pickup and storage process.
