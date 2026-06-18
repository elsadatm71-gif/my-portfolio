---
layout: project
title: "Epson Cargo Storing Robot"
description: "Autonomous cargo storing system using Epson T3-401S and computer vision."
permalink: /projects/epson-robot/
categories:
  - Robotics
  - Mechatronics
project_folder: "epson-robot"
featured_image: "/assets/projects/epson-robot/cover.png"
models:
  - file: "/assets/projects/epson-robot/epson-adapter.glb"
    description: "Custom Epson T3 Adapter"

  - file: "/assets/projects/epson-robot/gripper.glb"
    description: "3D Printed Servo Gripper"
media:
  - file: "cover.png"
    title: "The System"
    description: "Epson cargo storing system."
   - file: "system-diagram.png"
    title: "System Architecture"
    description: "Overall system architecture."

  - file: "image1.jpeg"
    title: "Robot Setup"
    description: "Testing and calibration of the Epson T3-401S robot."

  - file: "demo-video.mp4"
    title: "Project Demonstration"
    description: "Full autonomous cargo storing operation."
    download_files:
  - name: "Complete Source Code"
    url: "/assets/projects/epson-robot/source-code.zip"
    description: "Python, Epson RC+ and Arduino source code."
    
---

## Overview

Autonomous cargo storing system using an Epson T3-401S SCARA robot and an ESP-32 CAM as a computer vision.

## Features

- ArUco marker detection
- Python communication
- Automatic cargo storing
- Real-time coordinate conversion
- Customized 3d gripper
- Arduino uno
