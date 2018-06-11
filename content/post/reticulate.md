+++
title = "Power of Reticulate"

date = 2018-05-20T00:00:00
lastmod = 2018-05-20T00:00:00
draft = false

tags = ["academic"]
summary = "Sync R API with Python API"

[header]
image = "headers/reti_header.png"
#caption = "Image credit: [**Academic**](https://github.com/gcushen/hugo-academic/)"
+++

It is been two weeks, since my last post about my GSoC selection. The first task assigned to me was writing a versatile install function for R API which will be at par in terms of functionalities of Python API. Earlier during my proposal preparation, I focussed on the need of configuration details required by databases such as **PostgreSQL**,**MySQL**,**SQLite**. For instance, they could be made available through, **configuration file (custom made by user or default file)** or in absence of this file, command the **Retriever** to use defaults from code base. 

Writing code for the above workflow, which will take into account, different databases, is indeed an immaculate task. To combat such complexities, one of mentors, suggested [Reticulate](https://rstudio.github.io/reticulate/articles/introduction.html) package. Its a package, that works wonders. Any package which resides in the world of Python and be imported in R and made to work in R environment.  After studying it theoretically, I was initially afraid of the execution speed, as it tries to combine two different worlds which dominate the space of Data Science. But, after giving it a number of trials, I fathomed that it executes pretty fast without any overhead, and can be incorporated directly to sync Python API and R API of **Data Retriever**. 

I studied code of **install function** of Python API deeply, to ensure that direct usage of its functions through **Reticulate** encompasses all the detailed tasks which are required by R API. After variety of executions for different database supports, I figured that, using **Reticulate** will be a boon. Synchronization of both the APIs requires minimal code and the pace of work has increased faster than ever. The Data Retriever might require an additional layer of detection of existance of Reticulate in the R environment as well. 

I expect to complete this task before coming weekend. In the coming week I plan to complete detection of **Python** in **Windows** machine for the Data Retriever. 