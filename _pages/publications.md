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

A surgical system aiming at better therapy for patients and less cognitive load for surgeons.

The hardware setup includes: the da Vinci surgical system, CMU-Boeing Blaser senor (a light-weighted laser scanner), stereo camera(Intel RealSense), forth sensor, motion simulation platform and phantom liver model.
![](https://changshiraine.github.io/images/dvrk_system.png )

The brief diagram of the system architecture:

![](https://changshiraine.github.io/images/dcrk_arch.png)

We built a motion simulation platform based on the open-source Stewart platform designed by Professor Ken Goldberg, to mimic the subtle motion or organ during the surgery due to the heartbeat and respiration of the patient.

![](https://changshiraine.github.io/images/dvrm_msp.jpg)

Demo Video
---------------

[![](https://changshiraine.github.io/images/research_front.jpg)](https://www.youtube.com/watch?v=6q6407emmPA)

Dermatological Tissue Deformation Modelling
======




