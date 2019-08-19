FROM jupyter/minimal-notebook

LABEL maintainer="OCIO Infrastructure Operations <jplis-sa@jpl.nasa.gov>"

USER root

# Install awscli 
RUN apt update -y && apt install python3-pip -y && pip install awscli boto bs4 requests

# Clone Access Key Generation repository

RUN install -d ~/.aws/scripts && cd ~/.aws/scripts && git clone https://github.jpl.nasa.gov/cloud/Access-Key-Generation.git

