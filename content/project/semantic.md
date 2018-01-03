+++
# Date this page was created.
date = "2016-04-27"

# Project title.
title = "Summarization of Document"

# Project summary to display on homepage.
summary = "Noun-Verb Graph"

# Optional image to display on homepage (relative to `static/img/` folder).
image_preview = "semantic.jpg"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["deep-learning"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# Does the project detail page use math formatting?
math = false

# Optional featured image (relative to `static/img/` folder).
[header]
image = "headers/semanticExtended.jpg"
#caption = "My caption :smile:"

+++

* **Introduction**
	* I was part of the team during my tenure at Mphasis NEXT Labs as a Software Engineer.
	* This project is aimed to summarize grammatically written English document by build a queriable directed graph based on semantics and context (i.e. Event and Action). The query on graph can retrieve information about action and its effect, and entity and its role. We adopted various NLP and text mining methodologies to build the graph and stored the graph in Neo4j for effective information retrieval.
	* This project involved usage of R and Python programming language, CoreNLP package for finding co-references among sentences, tokenization and POS tagging, Senna framework for Semantic Role Labelling, Semafor for frame-semantic parsing and Neo4j framework for graph querying.

* **My Role**
	* I implemented co-reference relationship builder using CoreNLP (which internally uses Stanford CoreNLP framework) for replacement of pronouns with their respective nouns.
	* I translated retrieved relationship between prominent nouns and verbs from the document pre-processing to Neo4j graph
	* (Team of two) We created a GUI in RShiny for a prototype demonstration
