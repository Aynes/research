FROM jupyter/minimal-notebook:latest

RUN conda install -c pytorch faiss-cpu
RUN mkdir .src/
# COPY requirements.txt .src/
# RUN pip install -r .src/requirements.txt

WORKDIR /home/jovyan/src