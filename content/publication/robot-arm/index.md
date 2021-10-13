---
title: "The Robot Arm"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin

date: "2021-08-01T00:00:00Z"
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

abstract: In the context of an international collaboration, a sub-millimeter positioning system is under development, the "Hive Tracker". Both the electronics and the embedded software being functional, the work presented here focuses on the use of the produced data as well as on optimization experiments. The tracker embeds two imperfect sensor types (optical and inertial), the purpose of this internship was to merge the best of each data type to improve dynamism, accuracy and stability of the system. This work took place in the following way, a first phase of study allowed getting used to the project tools and the realization of a simulator. The following phase was the implementation of a simulator, then a phase of design of a mechanical structure with constrained geometry. Finally, a characterization phase of the implemented tools was carried out. After this internship, the tracker has the theoretical tools set up and functional for a centimetric accuracy. The Kalman filter slightly attenuate noise of measurements. We can eventually hope to use only the data of the accelerometer in case of occlusion of photodiodes. The noise of the measurements being greater than expected, the rest of the team involved will be able to concentrate on the implementation of more specific tools.

# Summary. An optional shortened abstract.
summary: The Hive Tracker is a sub-millimetric 3D positioning system. It can works under occlusion, thanks to the sensor fusion it has embedded.

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'publication/hive-tracker/Internship_2018.pdf'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: 'publication/hive-tracker/defense-internship-4A.pptx'
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

This Master project was about the miniaturization of the Vive Tracker developpd by HTC. It allows sub-millimetric 3d positioning at scale, and embeds a 9DoF IMU with sensor fusion. The <a href="https://github.com/HiveTracker">repository</a> shows several developments and documented test bricks.

![alt text](hive-tracker.jpg "Vive Tracker vs Hive Tracker")

During this project, I had first simulate the Hive Tracker on a <a href="https://github.com/jumellet/Kalman-Filter/tree/Dev/Simulations">game engine</a>.


![alt text](sim.gif "Hive Tracker Simulation")

I have then implemented the mathematical principle of the HTC Vive localisation. We wanted to publish it in open source, we used Blender for 3D virtual representation.

![alt text](animation.gif "Real Time Positionning")
