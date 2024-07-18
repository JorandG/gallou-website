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

Abstract: Since the start of the space conquest, almost all spacecraft have been manufactured and assembled on the ground, then integrated into a launch vehicle for delivery into orbit. This ap­proach imposes significant limitations on the size, volume, and design of payloads. In addition, the size of the telescopes and antennas is intimately linked to their performance. Therefore, there is a need for improvement of the space assembly to get rid of these limitations. With the on -orbit assembly, the launched vehicle only embarks the modular components required for bigger and more complex structures which are then build via a robot. Truss assembly plays an important role when one needs to build strong and light structures. It also allows constructing complex structures from a simple one. It considerably reduces the amount of space and weight in the launch vehicle.

# Summary. An optional shortened abstract.
summary: Reinforcement Learning has been used to obtain a highly flexible path planning. In addition a new truss structure using bars and magnets has been proposed for large assembly. 

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'publication/master-thesis/NPU_Thesis.pdf'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: 'publication/master-thesis/defense-master-thesis.pptx'
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

#### Truss Assembly 

The joint at the assembly nodes is a crucial part. For a robotic assembly, it is the part that requires the most advanced techniques, but it could be facilitated with a well engineered process. Different are discussed for the assembly of mirrors and then magnetic joints are presented.

![alt text](assembly.png "Bars Assembly")

![alt text](final-assembly.png "Final assembly of 7 mirrors with the second design")

This design ease the assembly for the robot. First, the grasping is made using magnetization so no need for special grasping. There is no lost surface and the bars are lighter which is a very important consideration for an on-­orbit assembly where the payload is very costly. Then because of the symmetry of the bars, the assembly needs to care only about the orientation of the element on the z axis. Finally, this design can easily be printed in space same as the ”Trusselator” which considerably reduces the payload for big structures assembly.

#### Autonomous path planning 

The number of steps is the number of modifications of the joint angle. The DQL showed good results. With this Policy, the robot could find the optimal path to the target with the minimum number of 3 steps. Finally, that technique was kept to make the Pick and Place environment where the robot had to catch a ball with a magnetized end-effector and place it in another desired position. In the end, the robot did it with an average of 5 steps. 

![alt text](animation.gif "Autonomous planning")

