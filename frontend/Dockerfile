FROM node:8.17-alpine
WORKDIR /app
COPY . /app

ENV TODOS_API_ADDRESS=http://todos-api:8082
ENV PORT=8089
ENV AUTH_API_ADDRESS=http://auth-api:9000
RUN npm install
RUN npm run build
EXPOSE 8089
CMD npm start

#ENTRYPOINT ["node", "index.js"]
#COPY package.json /app
