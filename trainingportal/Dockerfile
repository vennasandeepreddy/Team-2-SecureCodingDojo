FROM node:lts-jessie
WORKDIR /home/node/app/
COPY . /home/node/app/
COPY package.json /home/node/app/
RUN cd /home/node/app && npm install
RUN cd /home/node/app && npm audit fix
EXPOSE 8081
ENTRYPOINT ["node","/home/node/app/server.js"]

