FROM node:18

WORKDIR /morphir
COPY . .

EXPOSE 18096

RUN apt-get update && apt-get upgrade -y && \
    apt-get install -y nodejs \
    npm

RUN npm install -g morphir-elm
ENTRYPOINT ./run.sh