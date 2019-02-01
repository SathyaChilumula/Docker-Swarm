#This is a Dockerfile will dockerize the simple python app into Docker image

FROM python:2.7-slim

MAINTAINER Sathya Chilumula

LABEL appname="app.py" \
      requirements="Redis and Flask" \
      version="1.0.0" \
      Releasedate="01-02-2019"

WORKDIR /app

ADD ./app <opt/clusterapp/app.py>

RUN pip install --trusted-host pypi.python.org -r requirements.txt

EXPOSE 80

ENV NAME world

CMD ["python", "app.py"]
