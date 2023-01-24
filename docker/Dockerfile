ARG NODE_VERSION="latest"
FROM node:${NODE_VERSION}

ARG DIRECTORY_PATH=/usr/src/app
ENV DIRECTORY_PATH=$DIRECTORY_PATH
RUN RUN apk add --update python make g++\  && rm -rf /var/cache/apk/*
WORKDIR $DIRECTORY_PATH

ENTRYPOINT ./docker/script.sh $DIRECTORY_PATH