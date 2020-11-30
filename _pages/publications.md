---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
<!---
{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}
--->

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

Research Projects
======

<!---
{% include base_path %}

{% for post in site.reseach reversed %}
  {% include archive-single.html %}
{% endfor %}
--->


Automatic Tumor Localization for Minimally Invasive Surgery 
======

[Project Website for more details](https://mrsdprojects.ri.cmu.edu/2020teama/documents/)
---------------

A surgical system aiming at better therapy for patients and less cognitive load for surgeons.

The hardware setup includes: the da Vinci surgical system, CMU-Boeing Blaser senor (a light-weighted laser scanner), stereo camera(Intel RealSense), forth sensor, motion simulation platform and phantom liver model.
![](https://changshiraine.github.io/images/dvrk_system.png )

A brief diagram of the system architecture:
![](https://changshiraine.github.io/images/dcrk_arch.png)

We built a motion simulation platform based on the open-source Stewart platform designed by Professor Ken Goldberg, to mimic the subtle motion or organ during the surgery due to the heartbeat and respiration of the patient.

![](https://changshiraine.github.io/images/dvrm_msp.jpg)

Demo Video
---------------

[![](https://changshiraine.github.io/images/research_front.jpg)](https://www.youtube.com/watch?v=6q6407emmPA)


Dermatological Tissue Deformation Modelling
======

During the production process of frozen pathological sections, the squeezing and strain caused by the slide would lead to deformation of the tissue. Modeling tissue processing biomechanics may identify aspects that contribute to errors in detecting tumors. 

Due to the homogenous texture of the tissue specimen, it’s hard to measure similarity with anatomical identifications during registration, thus we add artificial matte dye markers to the tissue. 

We operated iterative optimization of bidirectional blob matching and thin plate spline warping to obtain correspondence between artificial markers in the images shot on fresh tissue and those shot on frozen sections. The images below show an example of how the image matching improves comparing to naive method. (Due to medical data privacy, only a test on chicken skin is listed here. You may regard chicken skin placed on curvy surface as fresh tissue, while chicken skin placed on flat surface as frozen tissue section.)

![Naive test](https://changshiraine.github.io/images/bad.jpg)

![Our method](https://changshiraine.github.io/images/good.jpg)

We then use a customized calibrated RealSense camera to acquire the location information from the markers and get the deformation model. We are improving and verifying the model through collaboration with mathematicians of UPitts, who look into the problem from the computational perspective, by analyzing strain, Young’s modulus, etc.





