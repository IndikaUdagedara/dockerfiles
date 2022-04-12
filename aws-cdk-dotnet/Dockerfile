FROM ubuntu:18.04

RUN apt-get update

RUN apt-get install -y sudo curl gnupg zip

RUN curl -sL https://deb.nodesource.com/setup_17.x | sudo -E bash -
RUN curl -sO https://packages.microsoft.com/config/ubuntu/21.04/packages-microsoft-prod.deb
RUN dpkg -i packages-microsoft-prod.deb

RUN apt-get install -y apt-transport-https
RUN apt-get update
RUN apt-get install -y dotnet-sdk-6.0 nodejs
RUN npm install -g aws-cdk
