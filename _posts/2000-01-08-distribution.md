---
title: "distribution"
bg: darkmagenta
color: white
style: center
fa-icon: github
---

You can get phrapl in two ways. The easiest is to install the latest version from github:

`install.packages('devtools')`

`devtools::install_github('bomeara/phrapl')`

However, that only works for Mac and Linux machines. If you're using Windows, you can still run phrapl using Docker (this also works for Mac and Linux). Docker is like a lightweight virtual machine (lightweight because it can share many things between multiple virtual machines running on the same hardware).

See [here](https://docs.docker.com/docker-for-windows/) for how to install Docker on Windows.

Then you can use

`docker run -it --name bomeara/phydocker -v /Path/To/My/Folder:/data -p 8787:8787 bomeara/phydocker`

to run it as an RStudio Server. Change `/Path/To/My/Folder` to the absolute path to the folder you want access to (any subfolders will also be accessible). You can read and write to this in RStudio as the `/data` directory. In your web browser, go to `localhost:8787`, enter username and password (both are `rstudio`), to launch a version of RStudio that will run in your browser and have everything you might need. You might want to do `setwd("/data")` to make sure you're in the right directory. You can save any results or figures to this directory and it will still exist when you quit this instance.
