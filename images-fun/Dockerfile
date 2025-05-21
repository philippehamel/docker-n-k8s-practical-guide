FROM node:latest

WORKDIR  /app

COPY package.json /app

RUN npm install

COPY . /app

# Useless command but good practice
# docker run -p 3000:80 -d {id}
EXPOSE 80 

CMD [ "node", "server.js" ]