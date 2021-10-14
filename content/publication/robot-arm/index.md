---
title: "The EEZTbot with computer vision"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin

date: "2021-06-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
#publishDate: "2018-01-08T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["4"]

# Publication name and optional abbreviated publication name.
#publication: In *Wowchemy Conference*
#publication_short: In *ICW*

abstract: Open Sourced projects are growing and gaining more and more attention. The idea to share knowledge so that it profits to everybody is also the spirit of this project. Computer vision is a task that is highly interesting for a lot of robotics projects however beginners can be lost and not be able to use this powerful tool. This project aims to use the open source robot manipulator EEZYbot MK1 of daGHIZmo with computer vision. A first part is made in order to simply manipulate it with a joystick. Then computer vision is explained with object detection. And finally, computer vision will be added to the robot so that the end effector can follow an object //WIP.

# Summary. An optional shortened abstract.
summary: A robot arm manipulator using computer vision for control.

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: ''
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: ''
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
#projects:
#- example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
#slides: example
---

#### Installation

In order to manipulate the MK1 we used an arduino uno and a joystick as you can see on the following picture:

![alt text](installation.jpg "Robot arm controller with a joystick")

The servos are plugged on the PWN pins 5, 6, 9. And the joystick is plugged on the A0 and A1.

#### Conputer Vision

Steps are described on the github repository [EEZYbotComputerVision]("https://github.com/JorandG/EezybotMK1ComputerVision") so that the user can obtain the postion of an object in a square made with aruco markers as followed:

![alt text](cv.png "Object detection")
