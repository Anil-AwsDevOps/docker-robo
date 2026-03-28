FROM node:20
WORKDIR /app
COPY package.json .
COPY *.js .
RUN npm install 
ENV CATALOGUE_PORT=8080 \
    REDIS_URL='redis://redis:6379' \
    CATALOGUE_HOST=

CMD [ "node","server.js" ]
