FROM ubuntu:latest

RUN apt update && apt install -y pcs dnsutils bash-completion vim net-tools iproute2 vim iputils-ping  && rm -rf /var/lib/apt/lists*
RUN mkdir -p /var/log/cluster/
RUN touch /var/log/pcsd/pcsd.log