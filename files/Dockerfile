# Dockerfile

# Author       : gaurav
# Github       : https://github.com/Ydv95843
# Email        : ydvgaurav810@gmail.com
# Date         : 24-04-1999
# Main Language: Python

# Download and import main images

# Operating system
FROM debian:latest
# Main package
FROM python:3

# Author info
LABEL MAINTAINER="https://github.com/Ydv95843/zkPhisher"

# Working directory
WORKDIR /zkPhisher/
# Add files 
ADD . /zkPhisher

# Installing other packages
RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install python3-pip php openssh-client -y
RUN pip3 install -r files/requirements.txt --break-system-packages
RUN apt-get clean

# Main command
CMD ["python3", "pyphisher.py", "--noupdate"]

## Wanna run it own? Try following commnads:

## "sudo docker build . -t Ydv95843/zkphisher:latest", "sudo docker run --rm -it Ydv95843/zkphisher:latest"

## "sudo docker pull Ydv95843/zkphisher", "sudo docker run --rm -it Ydv95843/zkphisher"
