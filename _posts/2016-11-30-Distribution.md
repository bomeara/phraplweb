---
layout: post
title: Distribution
---

You can get phrapl in two ways. The easiest is to install the latest version from github:

```
install.packages('devtools')
devtools::install_github('bomeara/phrapl')
```

However, that only works for Mac and Linux machines. If you're using Windows, you can still run phrapl using Docker (this also works for Mac and Linux). Docker is like a lightweight virtual machine (lightweight because it can share many things between multiple virtual machines running on the same hardware).

See https://docs.docker.com/docker-for-windows/ for how to install Docker on Windows. Then open Kitematic and use the bomeara/phydocker image.
