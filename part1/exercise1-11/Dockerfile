FROM node:lts-alpine

RUN apk update && apk add git

WORKDIR /mydir

RUN git clone https://github.com/docker-hy/backend-example-docker.git

WORKDIR /mydir/backend-example-docker

RUN npm install

ENTRYPOINT [ "npm" ]

CMD [ "start" ]
