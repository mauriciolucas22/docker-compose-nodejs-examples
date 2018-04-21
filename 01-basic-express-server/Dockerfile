FROM ubuntu:latest

RUN apt-get update && apt-get install -y sudo curl && curl -sL https://deb.nodesource.com/setup_9.x | sudo -E bash - && sudo apt-get install -y nodejs

WORKDIR /app

ADD . /app

RUN npm install

EXPOSE 3000

CMD ["node", "app/server"]
