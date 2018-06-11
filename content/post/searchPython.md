+++
title = "Pursuit of Python"

date = 2018-05-20T00:00:00
lastmod = 2018-05-20T00:00:00
draft = false

tags = ["academic"]
summary = "Search Python in Windows"

[header]
image = "headers/python-header.png"
#caption = "Image credit: [**Academic**](https://github.com/gcushen/hugo-academic/)"
+++

Pursuit of Reticulate package in Windows is tricky than searching its installation in Ubuntu/Mac. Windows operating system has disintegrated structure for file storage. It also has different drives such as C,D etc. which can be the home for software installation. Over this layer of complicated file structure comes the different ways in which Python can be installed in the Windows OS. It can be a manual installation of **python.exe** or through frameworks such as **Miniconda**, **Anaconda**. This overlaying complications make the location of Python and its containing packages very unpredictable. Also, the search should be successful if the code in executed from the terminal or within IDE such as RStudio. I tried my best to go through proper research before writing my code for this convoluted **pursuit**. 

## Literature Survey
 
 * The current code for checking Reticulate installation in Windows adds all predicatable paths in which Python could have been installed taking into consideration manual as well as platform based installations. Then, these are added to the RStudio's environment PATH so that RStudio can locate **Reticulate**. The underlying disadvantage with this approach is the fact that, we cannot predict all the paths where Python could have been installed. During manual installation of Python, it could have been possible that the user gave its custom created directory as its location. This path, cannot be predicted for adding in the list of possible paths. Therefore, a more robust and flexibe approach is needed for this intricate pursuit.
 
 
 * **PythonInR** is a R package which allows the user to interact with Python from R environment. I studied its source code to understand how it is locating Python as its crucial step for the successfull package working. It has a function named **autodetectPython.R** which accomplishes this task. It tries to locate Python using **where** command in the terminal then filter the searches according to the "arch" of R version. Henceforth, it tries of locate dll file of Python for final connection
 
## Approach Implemented

The proposal I wrote for solving this problem used a command called **which** from the terminal. I tried to emulate the same process of **which** command of R. With the Windows 8, the terminal command was working like the command of R. The search needs to be carried out from the home directory containing the software to be searched. For example, if Reticulate is present in D drive, searching need to be started from the top most directory of the drive to find it. If the search begins from any other drive, say C, the search will be unsuccessful. 

But the trouble occurred, when I realised that, "which" terminal command was not present in Windows 10 and Windows 7 by default. Hence, I am currently using **where** command to carry out the search for Reticulate. I have checked that it is present in all the Windows. The best part of **where** command is that it can search for any entity irrespective of its current location. For example, if the current location is in C drive, an entity present in D Drive can be retrived. Therefore, it will take care of the different ways of Python installation as well as the complicated file structure of Windows.

