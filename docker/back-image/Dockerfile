FROM debian:bullseye
WORKDIR /infra
COPY . .
#Information in apt-get default
RUN apt-get update && apt-get install -y libaio1 libaio-dev ca-certificates build-essential apt-transport-https software-properties-common curl wget

#install nvm and node js 14.18.1
# RUN curl -sL https://deb.nodesource.com/setup_14.x | bash -
# RUN apt -y install nodejs=14.21.2-deb-1nodesource1
# RUN npm install npm

RUN curl -fsSLO https://nodejs.org/dist/v14.18.1/node-v14.18.1-linux-x64.tar.xz \
    && tar -xJf node-v14.18.1-linux-x64.tar.xz -C /usr/local --strip-components=1 \
    && rm node-v14.18.1-linux-x64.tar.xz

RUN node -v && npm -v

#install oracle client
RUN dpkg -i oracle-instantclient-basic_21.7.0.0.0-2_amd64.deb

#install oracle client
RUN apt-get install -y php7.4 php7.4-pgsql
     




# docker build -t pedroeduardo68/backendoraclephpnode:1 .