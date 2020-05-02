# Start with a Linux micro-container to keep the image tiny
FROM python:3.7.4-slim

# Document who is responsible for this image
MAINTAINER Alankrith Krishnan "alankrith.krishnan@nyu.edu"

# Set up a working folder and install the pre-reqs
WORKDIR /app
ADD pytorch-mnist/requirements.txt /app
RUN pip3 --no-cache-dir install -r requirements.txt

# Add the code as the last Docker layer because it changes the most
ADD pytorch-mnist/main.py  /app/main.py

# Run the service
CMD [ "python", "main.py" ]
