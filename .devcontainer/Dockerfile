ARG NODE_VER
FROM node:${NODE_VER}
RUN npm update -g npm

WORKDIR /home/node/app

RUN chown node:node .
RUN mkdir node_modules && chown node:node node_modules

COPY --chown=node:node ./frontend/package.json ./frontend/package-lock.json ./

USER node

RUN npm install

COPY --chown=node:node ./frontend ./

CMD ["npm", "run","dev"]