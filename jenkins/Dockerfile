FROM centos RUN yum repolist 
RUN yum install java-11-openjdk.x86_64 -y 
RUN yum install wget -y 
RUN wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat-stable/jenkins.repo 
RUN rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io.key 
RUN yum install jenkins -y 
RUN yum install /sbin/service -y 
RUN echo /etc/rc.d/init.d/jenkins start >> /root/.bashrc 
EXPOSE 8080

