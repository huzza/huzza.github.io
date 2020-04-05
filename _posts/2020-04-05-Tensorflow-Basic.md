---
layout: post
title: Tensorflow 2.0 >> Python Knowledge for Tensorflow 2.0
---

## Anaconda Python Environment
 
Commands to use conda to manage virtual environment 
```
$ conda create --name [env-name]
$ conda activate [env-name]
$ conda deactivate [env-name]
$ conda env remove --name [env-name]
$ conda env list
```

Examples:

```
$ conda create --name tf2 python=3.7
$ conda activate tf2
```

Use conda to install and manage python package:
```
$ conda install [package-name]
$ conda install [package-name]=X.X
$ conda update [package-name]
$ conda remove [package-name]
$ conda list
$ conda search [package-name]
```

If want to configure proxy for conda, add below context to ~/.condarc

```
proxy_servers:
    http: http://proxy-server:port
```

## pip package management
pip package command
```
$ pip install [package-name]
$ pip install [package-name]==X.X   # install pacakge with specified verison
$ pip install [package-name] --proxy=proxy_server:port  # install package with proxy
$ pip install [package-name] --upgrade
$ pip uninstall [pacakge-name]
$ pip list
```

## GPU & CUDA

Command to check GPU info
```
$ nvidia-smi  # command to list GPU info
```
Please note, the CUDA Toolkit and cuDNN version should match the Tensorflow version. Usually, in Tensorflow, it will specify which CUDA Toolkit and cuDNN needed