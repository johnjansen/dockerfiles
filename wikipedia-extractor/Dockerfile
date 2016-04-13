FROM python:2.7.10
MAINTAINER      johnjansen
RUN pip install --upgrade pip
RUN pip install progressbar
RUN pip install https://github.com/babilen/wp-download/zipball/master

ADD wpdownloadrc.conf /root/.wpdownloadrc

RUN mkdir /wikipedia
VOLUME ["/wikipedia"]

ENTRYPOINT ["wp-download", "--resume", "-v", "/wikipedia"]
