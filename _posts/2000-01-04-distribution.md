---
title: "distribution"
bg: lightyellow
color: black
style: left
fa-icon: github
---

You can get phrapl in two ways. The easiest is to install the latest version from github:

`install.packages('devtools')`

`devtools::install_github('bomeara/phrapl')`

However, that only works for Mac and Linux machines (if you get an rgl error on a Mac, try reinstalling [XQuarz](https://www.xquartz.org)). If you're using Windows, you can still run phrapl using Docker (this also works for Mac and Linux). Docker is like a lightweight virtual machine (lightweight because it can share many things between multiple virtual machines running on the same hardware).

See [here](https://docs.docker.com/docker-for-windows/) for how to install Docker on Windows. Docker for Windows requires 64bit Windows 10 Pro, Enterprise and Education (1511 November update, Build 10586 or later) and Microsoft Hyper-V.


Then you can use

`docker run -it -p 8787:8787 bomeara/phydocker`

to run it as an RStudio Server.

If you want to use a local folder, you can use

`docker run -it -v /Path/To/My/Folder:/data -p 8787:8787 bomeara/phydocker`

Change `/Path/To/My/Folder` to the absolute path to the folder you want access to (any subfolders will also be accessible). You can read and write to this in RStudio as the `/data` directory. In your web browser, go to `localhost:8787`, enter username and password (both are `rstudio`), to launch a version of RStudio that will run in your browser and have everything you might need. You might want to do `setwd("/data")` to make sure you're in the right directory. You can save any results or figures to this directory and it will still exist when you quit this instance.
