# devil1211/jupyter-notebook

This image(https://hub.docker.com/repository/docker/devil1211/jupyter-notebook) provides Jupyter-notebook installed with the latest version available.  

## Getting Started

### 1. create docker volume to make storage persistant 
```
      docker volume create myjupyter
```
### 2. launch docker container using patting and also using persistant volume 
```
   docker run -dit 
           - p 8888:8888 
           - v myjupyter:/tmp/jupyter
           -- name myjuputer
           devil1211/jupyter-notebook
```

### 3. Use browser to login  
```
      http://notebook_host_ip:8888
```
### 4. use the Initial login password for notebook
```
  dev
```

### Prerequisities

In order to run this container, you'll need Docker installed.

* [Windows](https://docs.docker.com/windows/started)
* [OS X](https://docs.docker.com/mac/started/)
* [Linux](https://docs.docker.com/linux/started/)

#### Volumes

* `myjupyter:/tmp/jupyter` - File location

## Built With

*jupyter lab
*python36
## Find Us

* [GitHub](https://github.com/deviljoshi)


## Authors
* **Devkishan Joshi** -  *Whole work* - (https://github.com/deviljoshi)

