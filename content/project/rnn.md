+++
# Date this page was created.
date = "2016-04-27"

# Project title.
title = "Solving Kinematics Word Problem"

# Project summary to display on homepage.
summary = "A Machine Learning and NLP based approach"

# Optional image to display on homepage (relative to `static/img/` folder).
image_preview = "rnn.png"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
#tags = ["deep-learning"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# Does the project detail page use math formatting?
math = false

# Optional featured image (relative to `static/img/` folder).
[header]
image = "headers/rnnExtended.png"
#caption = "My caption :smile:"

+++

* **Problem Description**
	* Machine is fed with a Kinematics word problem. It has to parse and understand the problem, and decide which equation will be required to solve the problem from the three equations-
		* s = u + a*t
		* v*v = u*u + 2*a*s
		* s = u*t + 0.5*a*t*t
	To achieve this, machine has to identify given entites such as velocity, displacement and time and also identify which entity has to be computed. 
* **Solution**
	* Existing related research papers concentrate on creating a question template to fit in the given entities and compute the missing one. But this prohibits the question solving capability of the machine to only free fall examples. Hence, I used RNN with LSTM network to train the machine with the questions and the label being the equation to solve it. I used NLP to make the understanding flexible as the machine has to identify details such as "at rest","initial velocity","final velocity","starting from rest" and also entites with different measuring  units such as metres per second, kilometers per hour etc.
* **Recognition**
	* I presented this work at Woman Who Code Conference held in Bangalore,India in March 2017 as a lightening talk speaker.