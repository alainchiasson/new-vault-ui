FROM node:latest
ARG PORT=3001

EXPOSE $PORT
ENV PORT=$PORT

WORKDIR /app
COPY package.json package-lock.json ./
RUN npm install
COPY . .
CMD ["npm", "start"]