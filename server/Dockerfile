FROM node:14.4.0-alpine
WORKDIR "/app"
COPY ./package.json ./
RUN npm install
COPY . .
RUN chown -R node:node /app/node_modules
CMD ["npm", "run", "start"]