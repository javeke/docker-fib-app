FROM node:14.14.0-alpine

USER node

RUN mkdir -p /home/node/client

WORKDIR /home/node/client

COPY --chown=node:node ./package*.json ./

RUN npm install

COPY --chown=node:node ./ ./

RUN npm run build


FROM nginx

EXPOSE 3000

COPY ./nginx/default.conf /etc/nginx/conf.d/default.conf

COPY --from=0 /home/node/client/build /usr/share/nginx/html