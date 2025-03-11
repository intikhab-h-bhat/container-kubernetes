FROM ubuntu

RUN apt-get update
RUN apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_18.x | bash -
RUN apt-get upgrade -y
RUN apt-get install -y nodejs

copy package.json package.json
copy package-lock.json package-lock.json
copy main.js main.js

Run npm install

ENTRYPOINT ["node","main.js"]
