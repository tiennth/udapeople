FROM node:13.8.0

RUN mkdir -p /usr/src/app/node_modules && chown -R node:node /usr/src/app

WORKDIR /usr/src/app

COPY package*.json ./

# USER node

RUN npm install

COPY . .

# RUN npm run build

EXPOSE 3030

CMD [ "npm", "run", "start" ]

