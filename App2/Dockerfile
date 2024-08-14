FROM node:12.18.3-alpine3.12

RUN npm install -g http-server

WORKDIR /LogisimWeb

COPY LogisimWeb/ .

EXPOSE 8001

CMD [ "http-server", ".", "-p", "8001" ]


