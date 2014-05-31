FROM pandrew/ubuntu-lts

RUN add-apt-repository ppa:fkrull/deadsnakes
RUN apt-get update
RUN apt-get install -y python2.6 python2.6-dev

ADD ./ /data
WORKDIR /data

CMD ["python", "-m", "SimpleHTTPServer", "8000"]
