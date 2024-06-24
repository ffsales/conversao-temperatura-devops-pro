FROM node:22-alpine3.19

# RUN apt-get update && \
#     apt-get install -y curl && \
#     curl -fsSL https://deb.nodesource.com/setup_current.x -o nodesource_setup.sh && \
#     bash nodesource_setup.sh && \
#     apt-get install -y nodejs

WORKDIR /app
COPY package*.json
RUN npm install
COPY . .
EXPOSE 8080
ENTRYPOINT ["node", "server.js"]