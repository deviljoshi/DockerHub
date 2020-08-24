FROM centos RUN yum install python36 -y 
RUN pip3 install jupyterlab 
RUN jupyter notebook --ip 0.0.0.0 --no-browser --generate-config 
COPY jupyter_notebook_config.json /root/.jupyter 
CMD jupyter notebook --allow-root --ip 0.0.0.0 --no-browser 
EXPOSE 8888

