FROM node:lts-alpine

RUN apk update && apk add git

WORKDIR /mydir

RUN git clone https://github.com/docker-hy/backend-example-docker.git

WORKDIR /mydir/backend-example-docker

RUN npm install

ENV FRONT_URL=http://localhost:5000

ENTRYPOINT [ "npm" ]

CMD [ "start" ]
