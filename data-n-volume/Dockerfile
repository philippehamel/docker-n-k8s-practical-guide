FROM node:14

WORKDIR /app

COPY package.json /app

RUN npm install

COPY . /app

EXPOSE 80

VOLUME [ "/app/feedback" ]

CMD [ "node", "server.js" ]

# docker build -t feedback-node .
# docker run -p 3000:80 -d --name feedback-app 
#   -v "feedback:/app/feedback"
#   -v "$(pwd):/app"
#   feedback-node