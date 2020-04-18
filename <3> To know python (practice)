FROM python:latest 
MAINTAINER Dr.Sungwon "drsungwon@khu.ac.kr"
COPY ./app
RUN apt-get update
RUN echo "this is a python web server container"
CMD ["python", “/app/webserver.py"]
EXPOSE 9000
