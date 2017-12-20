+++
# Date this page was created.
date = "2016-04-27"

# Project title.
title = "InfraGraf"

# Project summary to display on homepage.
summary = "Machine failure prediction"

# Optional image to display on homepage (relative to `static/img/` folder).
image_preview = "infragraf.PNG"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["demo"]

# Optional external URL for project (replaces project detail page).
#external_link = "http://example.org"

# Does the project detail page use math formatting?
math = false

# Optional featured image (relative to `static/img/` folder).
[header]
image = "headers/infragrafExtended.PNG"

+++

* **Introduction**
	* I was part of this project during my tenure at Mphasis NEXT Labs as an Intern and Software Engineer.
	* InfraGraf® is a Big Data complex event processing engine which enables enterprises to innovate and make strategic decisions regarding their technology infrastructure through actionable insights by correlation and causation analysis structured and unstructured data. It models enterprise technology infrastructure as complex systems consisting of interconnected servers, network devices, internet of things, industrial equipment etc. The powerful machine learning and graph theory based algorithms built into the platform identifies and predicts stand-alone as well as chain of events and incidents which could be related to system warnings, failures, outages, performance, availability and sub-optimal performances.

* **My Role**
	* Leveraging power of Apache Spark Framework - 
		* One of the data cleaning algorithms was taking more time than expected and an optimized approach for the same was crucial. I implemented the algorithm using Apache Spark in R programming language taking advantage of its distributed and parallel execution and robust implementation.
		* For execution on cluster mode, I used AWS EC2 instances and S3 for storage. I also wrote python script for automating the process of cluster creation, code execution and cluster termination.
		* It resulted in the decrease of the run time by 20 folds and was part of the product deployment.
	* Pattern Extraction from sequence data - 
		* Assigned to a team of two.
		* This is sub-project of the InfraGraf product. It is aimed at extracting all common patterns among given set event sequences with a minimum support and confidence. A common pattern is defined as a sequence which is subsequence among a defined minimum number of event sequences. Random walk based automata algorithm is built in C for this purpose. This algorithm is tested to give accurate results and implemented in real industrial applications.

