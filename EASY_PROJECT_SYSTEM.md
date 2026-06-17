# Easy Project Upload System

For every new project, use only one folder and one markdown file.

## Step 1 — Upload files

Create a folder:

```text
assets/projects/project-name/
```

Upload files inside it using simple names:

```text
cover.jpg
image1.jpg
image2.jpg
demo-video.mp4
report.pdf
code.zip
```

Avoid spaces in filenames.

## Step 2 — Create project page

Create:

```text
_projects/project-name.md
```

Use this format:

```markdown
---
layout: project
title: "Robot Project"
description: "Short description."
date: 2026-06-17
categories: [Robotics, Mechatronics]
project_folder: "project-name"

media:
  - file: "cover.jpg"
    title: "Final Photo"
    description: "Explain this image here."

  - file: "image1.jpg"
    title: "Design"
    description: "Explain this image here."

  - file: "demo-video.mp4"
    title: "Demo Video"
    description: "Explain this video here."

  - file: "report.pdf"
    title: "Report"
    description: "Download the project report."
---

## Overview
Write your project explanation here.
```

The website builds the full path automatically from `project_folder` + filename.
