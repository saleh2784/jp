FROM node:9
WORKDIR /app
COPY . .
RUN npm install
RUN npm run test
EXPOSE 3000
CMD ["npm", "run",  "start"]


