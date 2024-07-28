# ssh -i "docker-dep-example.pem" ec2-user@ec2-54-183-6-49.us-west-1.compute.amazonaws.com
FROM node:14-alpine

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 80

CMD ["node", "app.js"]