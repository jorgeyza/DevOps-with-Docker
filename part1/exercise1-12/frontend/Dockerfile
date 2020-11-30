FROM node:lts-alpine

RUN apk update && apk add git

WORKDIR /mydir

RUN git clone https://github.com/docker-hy/frontend-example-docker.git

WORKDIR /mydir/frontend-example-docker

RUN npm install

ENV API_URL=http://localhost:8000

ENTRYPOINT [ "npm" ]

CMD [ "start" ]
