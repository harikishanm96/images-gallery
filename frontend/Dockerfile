FROM node:20-alpine

WORKDIR /app

EXPOSE 3000

COPY package.json package-lock.json ./

# Install dependencies
RUN npm install --silent

COPY . ./

CMD ["npm", "start"]