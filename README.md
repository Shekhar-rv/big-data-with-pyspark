# big_data_with_pyspark
Spark and Python for Big Data with PySpark

This is the link to the docker image I have used:
```link
https://hub.docker.com/r/jupyter/pyspark-notebook
```

This is a link to further documentation if you want to update the docker settings such as user, rights etc:
```link
https://jupyter-docker-stacks.readthedocs.io/en/latest/using/common.html
```

## Prerequisites

Make sure you have VS Code and Docker installed.

## To get Jupyter Lab working

Run the following command:
```cmd
make run-notebook
```
This should get get the Jupyter Lab Notebook running on the same terminal and you should see a link like 
```link
http://127.0.0.1:8888/lab?token=***********************************
```
### Note: You should have a token generated at the end of the url, I have used `*` as a place holder.

If you click on the link it should open up on your web browser. 

If you need local files copied into the docker container, copy it into the following directory for ipynb files
```
docker -> pyspark_notebook -> work
```
And if you are copying data files such as xlsx or csv, copy it into the the data directory within the above mentioned directory.

### Note: 
1. Make sure you pull before you run the make command to build and run the docker container and also be sure to rerun the command if you copied over any local files as it needs to be copied over when the container is build.

2. Please save the notebook in Jupyter Lab and shutdown the kernel so that the latest changes are saved and please push them to git repo once done.

3. Note: If you need to install any new packages, you should add the name of the package along with the required version number to the requirements.txt file before you build and run the container.

# Happy Learning :)