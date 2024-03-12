FROM node:14
WORKDIR /usr/src/app
RUN apt-get update && apt-get install -y git
RUN git clone https://github.com/cristiklein/node-hostname.git .
RUN npm install
EXPOSE 3000
ENTRYPOINT ["npm", "start"]
