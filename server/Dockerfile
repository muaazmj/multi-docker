FROM node:14.14.0-alpine
WORKDIR /home/node/app
COPY ./package.json ./
RUN npm install
RUN mkdir -p node_modules/.cache && chmod -R 777 node_modules/.cache
COPY . .
CMD ["npm","run","start"]