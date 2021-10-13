---
title: "Master Thesis on Path Planning"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin

# Author notes (optional)
#author_notes:
#- "Equal contribution"
#- "Equal contribution"

date: "2021-07-06T00:00:00Z"
#doi: ""

# Schedule page publish date (NOT publication's date).
#publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["7"]

# Publication name and optional abbreviated publication name.
#publication: In *Wowchemy Conference*
#publication_short: In *ICW*

abstract: There is an increasing demand for fast drone deliveries for both consumer’s necessities and medical emergencies. All aircraft are subject to landing difficulties because of near-ground aerodynamic effects and complications with moving from air to land. In addition, for improving delivery, there have been many developments within space research aiming to reduce global cost. Reusable rockets are regarded as the future of space travel, however, numerous accidents have been observed during landing, making these rockets an unreliable resource for experimentation. The standard approach for both drone delivery and reusable rockets requires speed reduction before landing, as explained by the lack of precision of the embedded sensors combined with the fragility of the chassis. The landing shock thus needs to be attenuated to deform irremediably the frame structure. Therefore there is a need for improvement of landing approach for more reliability. The main research contents of this Master thesis cover different areas forthe development of a newly designed electric thrust vectored rocket that aims to incorporate a fast landing approach using this new benchmark system.

# Summary. An optional shortened abstract.
summary: The needs for fast drones with super-human capabilities has been applied for landing approach. 

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'publication/fast-landing/NPU-2018280049.pdf'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: 'publication/fast-landing/defense-master-thesis.pptx'
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

#### Drone Perception

This research proposed a way to generate accurate photorealistic dataset for a given landing pad. It was then possible to use it for supervised learning.

![alt text](camera-vision.jpg "Environment Landing Pad Generator")

The proposed [dataset generator](https://github.com/jumellet/landing-pad-dataset-generator) gave a way to feed the neural networks. It has now the ability to estimate accurately its position with a wide range of vision. Thanks to an appropriate landing pad shape, even seeing only part of the landing area permits the drone to descend.

#### Guidance and Control

For visual servoing, a multi-scale control is proposed where control sensitivity depends on drone altitude. The use of the neural network in a simulated environment multiplied by three the processing rate, the control is thus closer to real time. 

![alt text](drone-land.gif "Fast Landing Working Algorithm Demo")

#### Mechanical Landing Gear

For fast landing situations, the vertical speed is higher than standard descent. The research proposes a landing gears that absorbs more than ten times the kinetic energy of standard landing legs. A
**patent** is filed to protect the concept..

![alt text](landing-gear.jpg "Landing Gear Concept Evolution")
