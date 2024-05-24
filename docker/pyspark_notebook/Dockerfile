FROM jupyter/pyspark-notebook:latest

USER $NB_UID

WORKDIR /home/jovyan/packages
COPY docker/pyspark_notebook/requirements.txt /home/jovyan/packages/requirements.txt
RUN pip install -r requirements.txt

ENV ENV="dev"

WORKDIR /home/jovyan