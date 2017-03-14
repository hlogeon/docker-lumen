FROM mongo:latest

MAINTAINER Mahmoud Zalt <mahmoud@zalt.me>

#COPY mongo.conf /usr/local/etc/mongo/mongo.conf

COPY ./data /data/db

VOLUME /data

CMD ["mongod"]

EXPOSE 27017