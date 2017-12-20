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
	* Conversational user interfaces are becoming increasingly used for a variety of research needs.
	Some are voice-activated (such as Alexa, Siri, and Google Now), but many are text-oriented chatbots appearing as assistants in the context of a larger application. Text chatbots are being considered for providing help in using our products, but also for improving the legal research experience
	Given a set of case law and judge data, answer research questions using a text-oriented, conversational interface.
	For instance, if a user asks "List cases for Judge Lucy Koh", the system would respond with a list of cases where Judge Koh is listed as a presiding judge.

* **Test Cases**
	* U: List cases handled by Judge ADAMS
	*  B: THERE ARE 6 JUDGES with Llast name ADAMS and 2 JUDGES with FIRST NAME
	*  U: Last name ADAMS
	*  B: There are only 2 JUDGES with last name ADAMS who are currently on service with first name Henry Lee in Florida and John R in state of OHIO.
	*  U: The one in state of OHIO
	*  B: There were 0 cases handled by the judge


* **Team's Solution**
	* We trained DialogFlow with the provided data and then integrated it with Amazon Alexa as a medium of conversation. To accomplish this we used DialogFlow's Alexa Exporter and Amazon Developer Dashboard. After training DialogFlow with the data, we generated Alexa compatible files and then used these files to create a new skill for Alexa.
* **My Role**
	* I trained DialogFlow with help of the data by creating appropriate intents, entities and actions. 