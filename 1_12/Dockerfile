FROM ubuntu:24.04
RUN apt-get update && apt-get install -y ca-certificates libstdc++6 && rm -rf /var/lib/apt/lists/*
COPY --from=node:16-bullseye /usr/local/ /usr/local/
WORKDIR /usr/src/app
COPY package*.json ./
RUN npm install && npm install -g serve@14.2.4
COPY . .
RUN npm run build
EXPOSE 5001
CMD ["serve", "-s", "-l", "5001", "build"]
