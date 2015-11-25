FROM ubuntu:latest

RUN sed -i 's/archive.ubuntu.com/mirrors.digitalocean.com/g' /etc/apt/sources.list
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update && \ 
    apt-get -y upgrade && \
    apt-get install -y git-core vim tmux htop jq curl wget httpie && \ 
    apt-get clean && apt-get purge && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*