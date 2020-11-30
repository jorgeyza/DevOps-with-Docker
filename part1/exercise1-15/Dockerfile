FROM node:lts-alpine

RUN apk update && apk add git

WORKDIR /mydir

RUN git clone https://github.com/jorgeyza/anecdotes-fullstackopen.git

WORKDIR /mydir/anecdotes-fullstackopen

RUN npm install

ENTRYPOINT [ "npm" ]

CMD [ "start" ]
