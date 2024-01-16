---
title: "Dermatological Tissue Deformation Modelling"
# excerpt: "A deep learning based channel estimation solution, Spring 2019, Cisco Innovation Labs <br/><img src='/images/portfolio-2-small.png'>"
collection: portfolio

---

During the production process of frozen pathological sections, the squeezing and strain caused by the slide would lead to deformation of the tissue. Modeling tissue processing biomechanics may identify aspects that contribute to errors in detecting tumors. 

Due to the homogenous texture of the tissue specimen, it’s hard to measure similarity with anatomical identifications during registration, thus we add artificial matte dye markers to the tissue. 

We operated iterative optimization of bidirectional blob matching and thin plate spline warping to obtain correspondence between artificial markers in the images shot on fresh tissue and those shot on frozen sections. The images below show an example of how the image matching improves comparing to naive method. (Due to medical data privacy, only a test on chicken skin is listed here. You may regard chicken skin placed on curvy surface as fresh tissue, while chicken skin placed on flat surface as frozen tissue section.)

![Naive test](https://changshiraine.github.io/images/bad.jpg)

![Our method](https://changshiraine.github.io/images/good.jpg)

We then use a customized calibrated RealSense camera to acquire the location information from the markers and get the deformation model. We are improving and verifying the model through collaboration with mathematicians of UPitts, who look into the problem from the computational perspective, by analyzing strain, Young’s modulus, etc.
