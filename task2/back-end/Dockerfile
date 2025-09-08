FROM ubuntu:latest

WORKDIR /app

RUN apt-get update
RUN apt-get upgrade -y

COPY ./api.py /app/api.py

RUN apt-get install -y python3 python3-pip
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED
RUN pip3 install flask

CMD ["python3", "api.py"]