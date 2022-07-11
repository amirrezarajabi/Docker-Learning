FROM ubuntu

RUN apt-get update && apt-get -y install python3

COPY . /opt/source-code

ENTRYPOINT python3 /opt/source-code/app.py
