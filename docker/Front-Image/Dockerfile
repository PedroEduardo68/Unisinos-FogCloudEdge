FROM debian:bullseye
WORKDIR /infra
COPY . .

#Information in apt-get default
RUN apt-get update && apt-get install -y curl vim
RUN apt-get update && apt-get install -y \
    curl \
    ca-certificates \
    gnupg

RUN apt-get update && apt-get install -y curl xz-utils

RUN curl -fsSLO https://nodejs.org/dist/v14.18.1/node-v14.18.1-linux-x64.tar.xz \
    && tar -xJf node-v14.18.1-linux-x64.tar.xz -C /usr/local --strip-components=1 \
    && rm node-v14.18.1-linux-x64.tar.xz

RUN node -v && npm -v

# docker build -t pedroeduardo68/frontendnode14:1 .