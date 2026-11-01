FROM ubuntu

EXPOSE 5001

WORKDIR ./app

RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_16.x | bash && apt install -y nodejs && npm i

COPY . .
RUN npm i -g serve

RUN npm run build

CMD ["serve", "-s", "-l", "5001", "build"]
