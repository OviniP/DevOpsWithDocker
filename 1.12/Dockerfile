From ubuntu:22.04
RUN apt-get update
RUN apt-get -y install curl sudo
RUN curl -sL https://deb.nodesource.com/setup_16.x | bash
RUN sudo apt install -y nodejs

EXPOSE 5000
WORKDIR /app
COPY . .

RUN npm install
RUN npm run build
RUN npm install -g serve



CMD ["serve", "-s", "-l", "5000", "build"]