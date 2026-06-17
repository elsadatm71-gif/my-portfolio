# Easy Project Upload Guide

## Add a new project

1. Copy `_projects/template-new-project.md`.
2. Rename it, for example: `_projects/autonomous-mobile-robot.md`.
3. Create a folder for its files, for example: `assets/projects/autonomous-mobile-robot/`.
4. Put your images, short videos, PDFs, and code files inside that folder.
5. Edit the project file and change the paths.
6. Commit and push to GitHub.

## Recommended folder structure

```text
_projects/autonomous-mobile-robot.md
assets/projects/autonomous-mobile-robot/
  thumbnail.jpg
  image1.jpg
  demo.mp4
  report.pdf
  code/
    main.ino
    vision.py
```

## Important GitHub upload notes

- Keep normal images as `.jpg`, `.png`, `.gif`, `.webp`, or `.svg`.
- Keep short videos as `.mp4` or `.webm`.
- GitHub has file size limits. Avoid uploading very large videos. For big videos, upload them to YouTube or Google Drive and link/embed them.
- Use simple file names: no Arabic letters, no spaces, no special symbols. Good example: `robot-demo.mp4`.
- Do not edit `_layouts` every time. Only create one markdown file inside `_projects`.

## Simple project example

```yaml
---
layout: project
title: "Autonomous Mobile Robot"
description: "Vision-based robot that detects, picks, and places objects."
date: 2026-06-17
categories: [Robotics, ESP32, Computer Vision]
featured_image: "/assets/projects/autonomous-mobile-robot/thumbnail.jpg"
gallery:
  - file: "/assets/projects/autonomous-mobile-robot/image1.jpg"
    description: "Robot prototype"
  - file: "/assets/projects/autonomous-mobile-robot/demo.mp4"
    description: "Demo video"
download_files:
  - name: "Main Code"
    url: "/assets/projects/autonomous-mobile-robot/code/main.ino"
---

Write the project details here.
```
