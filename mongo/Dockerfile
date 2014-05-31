FROM pandrew/ubuntu-lts

# Install MongoDB.
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 7F0CEB10
RUN echo 'deb http://downloads-distro.mongodb.org/repo/ubuntu-upstart dist 10gen' | tee /etc/apt/sources.list.d/mongodb.list
RUN apt-get update
RUN apt-get install -y mongodb-org
RUN mkdir -p /data/db

WORKDIR /data

CMD ["mongod"]

EXPOSE 27017
EXPOSE 28017

