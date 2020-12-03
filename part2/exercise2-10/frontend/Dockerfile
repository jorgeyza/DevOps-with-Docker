FROM node:lts-alpine

RUN apk update && apk add git

WORKDIR /mydir

RUN git clone https://github.com/docker-hy/frontend-example-docker.git

WORKDIR /mydir/frontend-example-docker

RUN npm install

# Deleted ENV because it does not matter in the individual context of the image, it only matters when orchestrated with docker-compose

ENTRYPOINT [ "npm" ]

CMD [ "start" ]
