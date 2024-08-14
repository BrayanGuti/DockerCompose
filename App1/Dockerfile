FROM node:12.18.3-alpine3.12

RUN npm install -g http-server

WORKDIR /Sintaxify

COPY Sintaxify/ .

EXPOSE 8000

CMD [ "http-server", ".", "-p", "8000" ]


