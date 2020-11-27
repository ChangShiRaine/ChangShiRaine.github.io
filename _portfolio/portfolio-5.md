---
title: "Time-Varying DAGs with NOTEARS"
excerpt: "10-708 Probabilistic Graphical Models, Spring 2020, Carnegie Mellon University <br/><img src='/images/portfolio-5.png'>"
collection: portfolio

---

<!---
This is an item in your portfolio. It can be have images or nice text. If you name the file .md, it will be parsed as markdown. If you name the file .html, it will be parsed as HTML. 
--->

The gene expression of cells undergoes a large amount of transformation that can be linked to processes such as the development of progenitor stem cells or the transformation of healthy tissue into cancerous tumors. However, linking the changes of a single cell to other important dynamic processes occurring in surrounding cells/tissues is a non-trivial task. Cell development is oftentimes not synchronized within a single sample or tissue, introducing the need for flexibility in measuring temporal correlations. 

In order to solve these issues, time-based inference methods using graphical models that seek to account for the biological similarities among certain cells in addition their temporal dependencies have been introduced. The goal of this project is to optimize the Non-combinatorial Optimization via Trace Exponential and Augmented lagRangian for Structure learning (NOTEARS) framework ([Zheng et al., 2018](https://arxiv.org/abs/1803.01422)) for learning time-varying DAGs. 

We summarize our contributions as followed: 

1. We adapt the NOTEARS for the estimation of the graphical models using time-varying data.  
2. We introduce a theoretical modification to the existing DYNOTEARS framework to impose regularization on graph nodes that are close together in the time series.  
3. We compare several graph aggregation techniques to combine independent time series graphs into a static ground truth graph.  
4. We explore different time regularization techniques for combining independent, static graphs into dynamic graphs. 

![](/images/portfolio-5.png)

Figure: Accuracy of Temporally Regularized NOTEARS implementation. We implemented a dynamic Gaussian Bayesian network whose structure changed over time and assessed our algorithm’s ability to deduce the correct network structure over each time point. We utilized two networks: one “slowly-changing” network where each edge had a 10% of changing each time step and one faster changing network where each edge had a 50% chance of changing. The x-axis shows how “temporally smooth” our hyperparameterization forces the deduced graphs to be. The far left points represent no temporal smoothness penalization which is identical to using the original NO TEARS implementation on each time point independently.

[Download report here](http://changshiraine.github.io/files/10708_Final_Report.pdf)
