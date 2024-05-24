# big_data_with_pyspark
Spark and Python for Big Data with PySpark
https://hub.docker.com/r/jupyter/pyspark-notebook

So the image works flawlessly when running on its own.

What I'm trying to achieve is that:
1. I need a directory that needs to be copied over (can be blank or contain python notebooks)
2. I'm having an error trying to copy over the said directory
```error
PermissionError: [Errno 13] Permission denied: '/home/jovyan/.local'
```