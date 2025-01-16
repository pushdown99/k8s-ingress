FROM node:14
WORKDIR /app
#COPY package*.json ./
RUN npm install
COPY . .
RUN export $(cat .env | grep PORT | xargs)
EXPOSE $PORT
CMD ["node", "index.js"]