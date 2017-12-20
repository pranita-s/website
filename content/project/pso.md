+++
# Date this page was created.
date = "2016-04-27"

# Project title.
title = "Particle Swarm Optimization"

# Project summary to display on homepage.
summary = "An alternate to Differential Evolution tuner"

# Optional image to display on homepage (relative to `static/img/` folder).
image_preview = "pso.PNG"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["deep-learning"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# Does the project detail page use math formatting?
math = false

# Optional featured image (relative to `static/img/` folder).
[header]
image = "headers/psoExtended.jpg"
#caption = "My caption :smile:"

+++

* **Introduction**
	* The goal was to exibit the power of PSO with respect to DE as a tuner for SVM. For this comparison, we (a team of three) referred the paper "Easy over hard - A Case Study on Deep Learning" for the problem statement, data and performance metrics. DE has crossover and mutation functions for its implementation. We chose PSO for comparison as it has simpler implementation which revolves around the two update equations for velocity and position of particle. We wrote the code for PSO from scratch in Python. 

* **Conclusion**
	* After testing PSO, we found that its performance metrics are at par with those of DE. But the time it takes for convergence is more, hence it is slightly slower than DE. It can be concluded that PSO can be used instead of DE, depending on the usecase and the important factors.

* **My Role**
	* I contributed in the implementation of PSO algorithm in Python.
	* Presentation for the same can be seen at - https://docs.google.com/presentation/d/1FCd6igOw26W61A8BTVw7EHkDMXfhQ50d6YtcpuwGTMc/edit?usp=sharing.