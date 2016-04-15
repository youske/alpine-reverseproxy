# alpine linux with nginx reverse proxy
#
FROM youske/alpine-std:latest
MAINTAINER youske miyakoshi <youske@gmail.com>

ENV MEMORY_SIZE=1024 \
    PACKAGE=nginx \
    PATH=$PATH

RUN apk update --no-cache && apk add ${PACKAGE} --no-cache

EXPOSE 80 8088

ENTRYPOINT ["switch","shell=/bin/bash","--","nginx"]
