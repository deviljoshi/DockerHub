# Jenkins

This image(https://hub.docker.com/r/devil1211/jenkins)provides Jenkins installed with the latest version available.  

## Getting Started

### 1. create docker volume to make storage persistant 
```
      docker volume create myjenkins
```
### 2. launch docker container using patting and also using persistant volume 
```
   docker run -dit 
           - p 8080:8080 
           - v myjenkins:/var/lib/jenkins
           -- name myjenkins
           devil1211/jenkins:v1
```
### 3. Get the Initial login password of Jenkins 
```
  docker exec 
         myjenkins
         cat /var/lib/jenkins/secrets/initialAdminPassword
```
### 4. Use browser to login  
```
      http://jenkins_host_ip:8080
```

### Prerequisities

In order to run this container, you'll need Docker installed.

* [Windows](https://docs.docker.com/windows/started)
* [OS X](https://docs.docker.com/mac/started/)
* [Linux](https://docs.docker.com/linux/started/)

#### Volumes

* `/var/lib/jenkins` - File location

## Built With

* java (OpenJDK 64-Bit Server VM 18.9)
* jenkins [https://pkg.jenkins.io/redhat-stable/]
## Find Us

* [GitHub](https://github.com/deviljoshi)


## Authors
* **Devkishan Joshi** -  *Whole work* - (https://github.com/deviljoshi)

