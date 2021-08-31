FROM node:16-alpine as base
WORKDIR /src
COPY package*.json ./

#from base as production
#env node_env=production
#run npm ci
#COPY ./*.js ./
#CMD ["node", "index.js"]

FROM base as dev
RUN apk add --no-cache bash
RUN wget -O /bin/wait-for-it.sh https://raw.githubusercontent.com/vishnubob/wait-for-it/master/wait-for-it.sh
RUN chmod +x /bin/wait-for-it.sh

ENV NODE_ENV=development
RUN npm install
COPY ./*.js ./
EXPOSE 3000
CMD ["npm", "start"]
