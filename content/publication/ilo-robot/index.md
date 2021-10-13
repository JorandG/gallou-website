---
title: "The Educational Robot: ilo"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Simon Le Berre

# Author notes (optional)
#author_notes:
#- "Equal contribution"
#- "Equal contribution"

date: "2020-01-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
#publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["0"]

# Publication name and optional abbreviated publication name.
#publication: In *Wowchemy Conference*
#publication_short: In *ICW*

abstract: This platform is an open source meccanum vehicle. Meccanum wheels allow ilo to have 3 real degree of freedom on the ground. The robot is firstly build for educative purpose from elementary school, with introduction to algorithms. As an open-source platform, embedding powerfull components, it is also possible to use it for any other robotic project.

# Summary. An optional shortened abstract.
summary: ilo is a platform firstly developed to enable algorithmic developement at elementary school. It is programmable with the easiest way, simply taking photo of the planned path.

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
projects:
#- example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
#slides: example
---

![alt text](cad-print.JPG "ilo CAD to Printed")

#### System Architecture

The robot embeds common and open source components to be easily made.

![alt text](architecture.jpg "ilo Architecture")

The arduino is simply there to control the motors via the RAMPS 1.6, which is the motor shield. As a slave, it responds to a serial command of speed intensity on both translation and rotation possible on the ground. The raspberry is the master and controls all the actuators.

#### Mechanical Design

The robot manufacturing tries to take advandage of 3D printing. This would allow for a greater sharing of the project.

![alt text](facettes-print.JPG "ilo from every angle")

As the project aims to be open source, we try to make the robot fully 3D printable. [Here]("https://github.com/jumellet/ilo-bot/tree/main/parts") can be found the differnet parts.

![alt text](wheels.jpg "ilo Meccanum Wheels")

The Meccanum wheels are the key part of the robot, and enable it to have 3 degrees of liberty on the ground.

#### Elementary Programming

Our goal to introduce algorithm theory from the youngest age. We provide an easy way to learn how to structure computer code and execute it.

![alt text](arrows.jpg "ilo Image Detection")

Our system has the particularity to allow children to code without a computer. With a pencil and a sheet of paper, you can start to code the robot's movements. The idea is to open the doors of programming as soon as possible and to as many people as possible. Verification the programming of the robot path is done with the application. It is simply a matter of taking a picture and ilo will start its journey.