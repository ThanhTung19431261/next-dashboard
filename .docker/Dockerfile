# Use the official Node.js 20 image as the base image
FROM node:20-alpine
WORKDIR /usr/app
RUN npm install -g pnpm
COPY ../package*.json ./
RUN pnpm install
COPY ../ ./
# RUN pnpm build
EXPOSE 3000
ENTRYPOINT [ "pnpm", "dev" ]