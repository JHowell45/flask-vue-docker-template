# build stage
FROM node:lts-alpine

WORKDIR /app

COPY package*.json ./
RUN npm install

ENV NODE_ENV=production

COPY . .
RUN npm run build

#RUN rm -rf ./src
#RUN rm -rf ./build


EXPOSE 8080
CMD [ "yarn", "serve" ]