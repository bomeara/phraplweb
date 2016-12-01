---
title: "distribution"
bg: purple
color: white
style: center
fa-icon: github
---

You can get phrapl in two ways. The easiest is to install the latest version from github:

`install.packages('devtools')`

`devtools::install_github('bomeara/phrapl')`

However, that only works for Mac and Linux machines. If you're using Windows, you can still run phrapl using Docker (this also works for Mac and Linux). Docker is like a lightweight virtual machine (lightweight because it can share many things between multiple virtual machines running on the same hardware).

See https://docs.docker.com/docker-for-windows/ for how to install Docker on Windows.

Then you can use

`docker run -it --name bomeara/phydocker -v /Path/To/My/Folder:/data -p 8080:8080 bomeara/phydocker`

to run it as an RStudio Server (username and password are both `rstudio`) with access to your current folder. Within
